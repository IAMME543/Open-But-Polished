# System State Store
Attached to the settings app there needs to be a definition of where state is stored.

For variable state it is simple, the daemon which controls that state is the source of truth.
    eg: NetworkManager is the source of truth for the wifi state
    eg: Power Profiles Daemon is the source of truth for the current power profile

For non-variable state and stuff we will have to implement ourselves. We should use a file based data store.
    Eg: ~/.config/state/appaerance/theme contains the last recorded change in state. Which should only be updated by an elevated program. In this example that program could be my toggle-theme bash script in my dotfiles. Currently it does not remember state, it just takes in the theme and updates all the different consumers of the system theme state(gtk, qt, specific app configs). The source of truth should be written to a read only file as the source of truth.

    Eg: A similar thing could be implemented for a system accent colour. A script or deticated daemon is told what to update the accent colour to, it writes that to the store file and then goes and informs all the consumers of the state.