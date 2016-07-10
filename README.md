# Synergy for Haiku

![Synergy for Haiku](SynergyHaiku.png "Synergy for Haiku")

Synergy for Haiku is a [Synergy](http://symless.com) client for the [Haiku Operating System](http://haiku-os.org).

Synergy allows a central machine running the Synergy server to share its Keyboard and Mouse across multiple systems running the client as if they were one desktop.

## Limitations
  - Synergy for Haiku is only a Synergy client at this time
  - Some minor bugs still exist in the keymap translation

## Features
  - Import and save files from GitHub, Dropbox, Google Drive and One Drive
  - Drag and drop files into Dillinger
  - Export documents as Markdown, HTML and PDF

## Compiling
Simply run ```make``` under Haiku

## Configuration
  Create a configuration file at ```~/config/settings/synergy_settings```
  
  ```ini
  enable = true
  server = 192.168.1.101
  server_keymap = "X11"
  ```
### Options
  * **Enable**: Enable the client (true|false)
  * **Server**: Server address
  * **Server_keymap**: Keymap of the Synergy Server (X11)
  
## Manual Installation
Copy the synergy_client input add-on to the non-packaged add-ons directory ```~/config/non-packaged/add-ons/input_server/devices/```
