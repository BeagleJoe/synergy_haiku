# Synergy for Haiku

![Synergy for Haiku](SynergyHaiku.png "Synergy for Haiku")

Synergy for Haiku is a [Synergy](http://symless.com) client for the [Haiku Operating System](http://haiku-os.org).

Synergy allows a central machine running the Synergy server to share its Keyboard and Mouse across multiple systems running the client as if they were one desktop.

## Release notes 0.3-1
  - Fixed x86-64
  - enabel/disable copy&paste feture
  - Key Mapping (cntl+alt+arrows) for x11
  - sticky keys

## Now Package available:
Package available: https://depot.haiku-os.org/ or in HaikuDepot app.

## Limitations
  - Synergy for Haiku is only a Synergy client at this time
  - Some minor bugs still exist in the keymap translation
  - For now, client name is always "haiku"
  - SSL / TLS is not currently supported and must be disabled on the server
  - Copy / Paste feature have some issues

## Compiling
Simply run ```make``` under Haiku (x86 and x86-68 tested)

## Configuration
  Create a configuration file at ```~/config/settings/synergy```
  
  ```ini
  enable = true
  server = 192.168.1.101
  server_keymap = "X11"
  enableCLipboard = false
  ```
### Options
  * **enable**: Enable the client (true|false)
  * **server**: Server address
  * **server_keymap**: Keymap of the Synergy Server (X11|AT)
  * **client_name**: Name of client (string, "haiku" default)
  * **enableCLipboard**: Enable/Disable copy paste feature (false recomended)
  
## Manual Installation
Copy the synergy_client input add-on to the non-packaged add-ons directory ```~/config/non-packaged/add-ons/input_server/devices/```

## License
Synergy for Haiku is released under the same license as uSynergy (MIT)

## Thanks
Thanks to all of those individuals who have made major contributions to Synergy for Haiku.

* Axel Dörfler (ATKeymap)
* Stefano Ceccherini (wrapper)
* Jérôme Duval (Keymap)
* Alex Evans (uSynergy)
* Jessica Hamilton (wrapper)
* Ed Robbins (wrapper)
* and the HaikuPorts team!

