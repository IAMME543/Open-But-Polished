# Open But Polished Shell
In this document, a shell is defined as the system UI and architecture that orchestrates all of the software and tools the user should not have to touch. This means gui wrappers for NetworkManager and BlueZ as well as some menu to open apps and get information for the system.

For the shell of OpenButPolished, rather than reimplementing everything we will simply orchestrate existing tools and organise them from a central place([SetThings](https://github.com/IAMME543/Set-Things) and possibly a daemon). The tools specifically that we are orchestrating incude:



### UI stuff
* Sway WM
* Waybar
* Fuzzel

Which is all being configured in my [dotfiles](https://github.com/IAMME543/dotfiles) repository.

## System daemons
* Flatpak
* Network Manager
* BlueZ
* Power Profiles Daemon / Upower
* Pipewire

and then a lot of undetermined things over the `org.freedesktop` dbus.
