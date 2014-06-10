GPX to Map - vBulletin Product
==============================

GPX to Map is a vBulletin Product which will display .gpx files attached
to a post as a Google Map.

This Product has been tested with the following versions of vBulletin:
* 4.2.2 Patch Level 1

![GPX to Map](https://taeram.github.io/media/gpx-to-map-vbulletin.png)

# Features

If a post has a .gpx file attached to it, a map automatically appears to the right of the post:
* The points in the GPX file are extracted and placed on the map
* The map has a slider which can be dragged back and forth to "play" through the points on the map
* The date and time of the currently selected point is displayed in your local timezone
* Clicking the "Toggle Map Size" link switches the map between default and full sized
* Customizable map marker and link colours

For what's changed between releases, see the [CHANGELOG](CHANGELOG.md).

# Licensing
This code is distributed under the [MIT License](LICENSE).

# Installation / Upgrading
Download the latest release from the [Releases](https://github.com/taeram/gpx-to-map-vbulletin/releases) tab,
and unpack it on your computer.

Next, to install or upgrade the product:
* Login to the Admin Control Panel in your vBulletin server
* In the sidebar, click "Plugins & Products"
* In the sidebar, click "Manage Products"
* Scroll to the bottom of the page, and click "Add/Import Product"
* Click the "Choose File" button, and select the product.xml you unpacked earlier.
* If upgrading, be sure and select "Yes" to the "Allow Overwrite" option
* Click the "Import" button

# Settings

To configure the settings for GPX to Map:
* Login to the Admin Control Panel in your vBulletin server
* In the sidebar, click "Settings"
* In the sidebar, click "Options"
* From the "Settings to Edit" list, select "GPX to Map Options"
* Click "Edit Settings"
* Customize the settings as you see fit, and click "Save"

Most settings have defaults, except for the "Google Maps API Key" setting, which
you'll need to get from the Google Developer Console:
* Sign in to https://developers.google.com/
* Create a project, give it a name
* Go to APIs & Auth => APIs
* Enable Google Maps JavaScript API v3
* Go to APIs & Auth => Credentials
* Generate a Public API access "Browser Key"
* Back in vBulletin, open up the "GPX to Map Options" page
* Paste the key from Google into the "Google Maps API Key" box
* Click "Save"
