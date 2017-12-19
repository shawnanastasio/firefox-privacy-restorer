firefox-privacy-restorer
========================
A script to modify your Firefox preferences to disable telemetry, built-in advertisements, and data collection anti-features.

The changes this script makes can all be done manually via `about:config`, but this becomes tedious and impractical across multiple machines and Firefox installations.

Licensed under the MIT license. See LICENSE for more information.

Why?
---
Mozilla has recently made some decisions that many members of the community believe have betrayed their trust in the browser, and as a result the need for a privacy-respecting alternative was created. After some investigation, I learned that it was possible to achieve this goal without switching browsers by modifying some settings in `about:config`, and decided to create this script to automate the process.

This is still a work in progress, and feedback and other contributions are welcome.

Usage
-----
### Linux/macOS
To start, first clone the repository
```
git clone https://github.com/shawnanastasio/firefox-privacy-restorer
cd firefox-privacy-restorer
```
Next, simply call the script with python3 (you may need to download this from your package manager).
```
$ python3 firefox-privacy-restorer.py
```
If you are prompted to select a profile, simply enter its number (or leave blank for all) and press enter.
```
$ python3 firefox-privacy-restorer.py
Detected multiple firefox profiles.
Please pick which one(s) to use:
1. /home/shawnanastasio/.mozilla/firefox/3pa6py6n.default/
2. /home/shawnanastasio/.mozilla/firefox/c4pnubpd.default/
Choice (1-2) [all]: 1

Firefox user.js profile successfully updated! Please restart Firefox to apply changes.
```
After the script is done running, simply restart Firefox to apply the changes.

### Windows

Windows support is currently untested, but should work. Standalone .exe binaries are planned in the future.