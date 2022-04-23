# Google App Launcher

Simple access to Google Applications with a tool bar button

> [Original Repository](https://github.com/asolkar/ffx-addon-gglappbtn)

> [Get on AMO](https://addons.mozilla.org/en-US/firefox/addon/google-app-launcher/)

Currently has links to popular Google applications in a 3x3 grid. There is some customization support to pick the 9 apps and the order.

## Supported apps

* `gmail`: Gmail
* `gcal`: Calendar
* `gsheets`: Sheets
* `gdrv`: Drive
* `gnews`: News
* `gdoc`: Docs
* `gphotos`: Photos
* `gmaps`: Maps
* `gmeet`: Meet
* `gpod`: Podcasts
* `gplay`: Play
* `gytube`: YouTube
* `gmsgs`: Messages
* `gduo`: Duo
* `ghang`: Hangouts
* `gcont`: Contacts
* `gtrans`: Translate
* `gkeep`: Keep
* `gmusic`: Music
* `gvoice`: Voice
* `gslides`: Slides
* `gclass`: Classroom
* `ggroups`: Groups
* `google`: Search

## Known issues

* Unit tests not working
* Possible conflict with icons png used from Google's assets.

## How to Debug (Windows)

- Make sure JPM and Git Bash are installed.
- Create a test profile, mainly to disable Extension Signing.

		/C/Program\ Files/Nightly/firefox.exe \
    		--profile /C/Users/.../ffx-addon-prof


-  In the Firefox window that opens, open about:config and set xpinstall.signatures.required to false
- Navigate into the add-on directory and use the following to invoke debug run:

		jpm run --binary /C/Program\ Files/Nightly/firefox.exe \
    				--profile /C/Users/.../ffx-addon-prof --debug


