# iTunesPlayCountFromLastFM
I used the Javascript for Automation on Mac (JXA) to create an iTunes script, that pulls your personal last.fm play counts.

## System Requirements
This code works only on MAC OS X Yosemite (10.10), due to Javascript being introduced just to this platform, yet. I will upload a build release for earlier OSX versions.

## Usage

### Build/Run
**The script causes a timeout when run directly in iTunes!**

The script is written in vanilla JavaScript and cannot be directly opened in Script Editor. To run the script you can use the shell command `osascript -l Javascript [file_name]` or build a .scpt file with `osacompile -l JavaScript -o [script_name].scpt [file_base_name].js` and run that in Skript Editor or directly in iTunes

### Manual
1. Select the tracks you like to sync in iTunes.
2. Start the script.
3. You are asked to input your last.fm username.
4. The scripts runs through all the selected tracks.

## Useful Resources
1. [JavaScript for Automation Release Notes](https://developer.apple.com/library/mac/releasenotes/InterapplicationCommunication/RN-JavaScriptForAutomation/#//apple_ref/doc/uid/TP40014508-CH109-SW11)
2. ['Getting Started with JavaScript for Automation on Yosemite'
by Alex Guyot](http://www.macstories.net/tutorials/getting-started-with-javascript-for-automation-on-yosemite/)
3. [JXA-Cookbook](https://github.com/dtinth/JXA-Cookbook)