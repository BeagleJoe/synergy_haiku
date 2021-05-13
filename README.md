# Synergy / Barrier client for Haiku-OS

![Synergy for Haiku](SynergyHaiku.png "Synergy for Haiku")

Synergy / Barrier for Haiku is a [Synergy](http://symless.com) / [Barrier](https://github.com/debauchee/barrier) client for the [Haiku Operating System](http://haiku-os.org).

Synergy / Barrier allows a central machine running the Synergy or Barrier server to share its Keyboard and Mouse across multiple systems running the client as if they were one desktop.

## Release notes 0.3-1
  - Fixed x86-64 architecture compilation
  - enabel/disable copy&paste feature
  - Bugs in Key Mapping (cntrl+alt+arrows) for x11
  - sticky keys

## Release notes 0.3-2
  - Add support for Barrier
  - Add keys support in Key Mapping 

## Now Package available:
Package available: https://depot.haiku-os.org/ or in HaikuDepot app.

## Limitations
  - Synergy/Barrier for Haiku is only a Synergy/Barrier client
  - SSL / TLS is not currently supported and must be disabled on the server
  - Copy / Paste feature have some issues; disable it is recommended

## Compiling
Simply run ```make``` under Haiku (x86 and x86-64 tested)

## Configuration
  Create a configuration file at ```~/config/settings/synergy```

  ```ini
  enable = true
  server = 192.168.1.101
  server_keymap = "X11"
  enableCLipboard = false
  use_barrier = false
  ```
### Options
  * **enable**: Enable the client (true|false)
  * **server**: Server address
  * **server_keymap**: Keymap of the Synergy Server (X11|AT)
  * **client_name**: Name of client (string, "haiku" default)
  * **enableCLipboard**: Enable/Disable copy paste feature (false recomended / false as default)
  * **use_barrier**: use Barrier(true|false)

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
* Nahuel Tello (fixes & hpkg)
* Fredrik Modéen (fixes & Barrier support)


