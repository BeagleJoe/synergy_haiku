# Synergy for Haiku

![Synergy for Haiku](SynergyHaiku.png "Synergy for Haiku")

Synergy for Haiku is a [Synergy](http://symless.com) client for the [Haiku Operating System](http://haiku-os.org).

Synergy allows a central machine running the Synergy server to share its Keyboard and Mouse across multiple systems running the client as if they were one desktop.

## Limitations
  - Synergy for Haiku is only a Synergy client at this time
  - Some minor bugs still exist in the keymap translation
  - For now, client name is always "haiku"
  - SSL / TLS is not currently supported and must be disabled on the server

## Compiling
Simply run ```make``` under Haiku

## Configuration
  Create a configuration file at ```~/config/settings/synergy```
  
  ```ini
  enable = true
  server = 192.168.1.101
  server_keymap = "X11"
  ```
### Options
  * **enable**: Enable the client (true|false)
  * **server**: Server address
  * **server_keymap**: Keymap of the Synergy Server (X11|AT)
  * **client_name**: Name of client (string, "haiku" default)
  
## Manual Installation
Copy the synergy_client input add-on to the non-packaged add-ons directory ```~/config/non-packaged/add-ons/input_server/devices/```
