# Apps

Install, Uninstall, Manage App and App data, settings, configs, etc... in one place.

Store and App, Launcher management tools.

Planning to support:
- Flatpak
- AppImage
- Distrobox

Additionally features:
- Editting Launchers
- Managing Startup Launchers.
- etc.

Let's anyone use Linux easily and manage apps easily in one place, easy to use and understand by normal everyday people.
You are on a Fedora? But have `.deb` package? No problem, doule click on it, and install it on distrobox.

We have two main tabs, "Store" and "Installed", installed tab has the same layout as Gnome settings or similar. 
Basically have two panes, left pane have a categories and under them buttons.

Categories can be:
- Flatpak
- Distrobox
- AppImage

Under flatpak category, we can have flatpak remotes on the left pane again.\
And under Distrobox category we have distroboxes basically.\
And under the AppImage Category, we can have the AppImage folders, and one for randomly found appimages in the system.

Each category at the bottom can have a button that says "Add Remote", "Create Distrobox", "Add Library" etc.

When we click on a flatpak repo, on the right pane we see a hero that says more about the remote, and under it have the app list installed from that repo.\
When we click on a distrobox, on the right pane we see a hero that says more about the distrobox, have actions like, start/stop it, or open it in terminal, and also at the bottom of it we also have list of exportable app in the distrobox.\
When we click on a appimage library, on the right pane we see a hero that gives more info about the library, and we see appimages in that library...

Same patterns for flatpaks, distroboxes and appimages basically.

We should also how the detailed info about app size, and its data size, and cache size. etc.

Some more notes:
- Distrobox should by default include GPU integration and create a custom isolated home folder for each distrobox.
- AppImages should have portable home folders by default.
- Even thought app is not using `.cache` for cache, we should still have a seperate button to delete cache.
- Take Android app management as an example, clear cache, clear appdata, uninstall, uninstall but keep data (might clear cache).
- We should have warning banners in app detail pages for recommended actions: for example: we found an appimage inside the launchers, but its not placed in the appimages directory, we can have a little "Fix" button to move it on the banner.
- Editting launchers directly is unsafe, and should warn you.
- It might me better if startup launchers are executing the actual launcher, so if the launcher updates we dont have to keep an eye on two places.
- And we can detect when the targetted launcher is missing and also get rid of startup.
- We should also check repo of installed flatpaks, because remote can be removed after the app is installed. so we should also add to the remote list from install apps, and in the hero clearly state that repo doesnt exists anymore and the app is an oprhan. unless flatpak already gives us the remote of the apps by itself.
