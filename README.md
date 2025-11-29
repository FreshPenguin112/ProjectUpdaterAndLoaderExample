Dynamic project loader and updater project I made.

Project is under [projectupdater.pmp](projectupdater.pmp).

Should work good right out of the box, all you need to do:
- Make a public github repo, this repo(the one you're in right now) is used in the project for the demo.
- Edit the values in the stage/backdrop code to match your github username as well as the name of the repo you made.
- Make a file exactly named "projectloaderandupdater.versions.txt", it will have a no spaces comma seperated list of "version,fileName", these don't need to follow any pattern, just don't use commas in your file names. See [projectloaderandupdater.versions.txt](projectloaderandupdater.versions.txt) for an example. The project will display the version numbers in order of line number(you need to put each version and fileName pair on their own line).
- Upload the project files specified in projectloaderandupdater.versions.txt to your repo.
- Package this project via [my nodejs enabled packager](https://freshpenguin112.github.io/PenguinMod-Packager/) and package as an electron exectuable for your OS of choice(yes, this project needs nodejs support, no HTML or zip or any other methods will not work).
- You're done! You can freely distribute your executable to your users, they will automatically recieve any updates when connected to the internet.

Enjoy!

small note: this project will not work well for private cases, such as uploading your own project to itch.io to be paid for with money, since this requires a public github repo, as well the fact that the downloaded project files that you create are saved in the filesystem.

smaller note: just remembered that one of the things i use errors if not in a nodejs environment so you can't load project in browser editor to edit GitHub stuff, use my [nodejs editor](https://github.com/FreshPenguin112/NodeJs-Desk-Penguin) until i fix that. (use latest actions run artifact for either Windows or Linux).
