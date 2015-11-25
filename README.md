# iTunesPlayCountFromLastFM
I used the JavaScript for Automation on Mac (JXA) to create an iTunes script, that pulls your personal last.fm play counts.

## System Requirements
This code works only since MAC OS X Yosemite (>=10.10), due to JavaScript being introduced just to this platform, yet. I will upload a build release for earlier OSX versions.

## Usage

### Manual
1. Download the latest release, open the disk image and copy the app inside somewhere on your Mac (Scripts in the Folder `~/Library/iTunes/Scripts/`will be displayed in the iTunes script menu).
2. Select the tracks you like to sync in iTunes.
3. Start the script.
4. You are asked to enter your last.fm user name.
5. The scripts runs through all the selected tracks.

### Build/Run on Your Own
**The script causes a timeout when run directly in iTunes, when not build as an applet.**
The script is written in vanilla JavaScript and cannot be directly opened in Script Editor. To run the script you can use the shell command `osascript -l Javascript [file_name]` or build a .app file with `osacompile -l JavaScript -o [script_name].app [file_name]` and run that in Script Editor or directly in iTunes.

If you like to work in Sublime Text, I created a package for the Build System: [JXASublimeText](https://github.com/dharma-guardian/JXASublimeText).

## Helpful Resources
* ['Getting Started with JavaScript for Automation on Yosemite'
by Alex Guyot](http://www.macstories.net/tutorials/getting-started-with-javascript-for-automation-on-yosemite/)
* [JXA-Cookbook](https://github.com/dtinth/JXA-Cookbook)
* [JavaScript for Automation Release Notes](https://developer.apple.com/library/mac/releasenotes/InterapplicationCommunication/RN-JavaScriptForAutomation/#//apple_ref/doc/uid/TP40014508-CH109-SW11)
* [Building OS X Apps with JavaScript](http://tylergaw.com/articles/building-osx-apps-with-js) by [Tyler Gaw](http://tylergaw.com/)
