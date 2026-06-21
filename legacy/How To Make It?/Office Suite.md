# *"Office Suite*"
# Document Editor

Really what the first step in this suite will be is making *a* document editing app, rather than building an alternative for the entirety of office 365. Additionally I think we should not be looking at building a typesetting app. Something like [La Suite Numerique Docs](https://github.com/suitenumerique/docs) already has a scope I think we should mimick, where it focuses on content rather than on formatting. 

Now how do we build a document editing app?
So, we could throw together an infrastructure stack for everything we need (Auth, Yjs backend, database). Or, with this project being focused mainly on UX, we could just reused the affirmentioned solution to the problem? And just rebuild the frontend around our own [web components](https://github.com/mm750-school/OBP-Web-Components). It does only sound like a weekend project to shove the existing LSN frontend into a tauri app and see what happens?
