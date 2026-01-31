-----------------------------------------------------------------------
  E-mu Audity Updater
  (C) 2026 Ray Bellis
-----------------------------------------------------------------------

Important:

This updater is offered to the community as is, with no warranty.  It
has been tested on several Audity 2000 units without issue.  Its use is
at your own risk, and the author will not be responsible for any failure
of your device.

In the (unlikely) event of a failure, UK users are welcome to visit me
in person for help.

Instructions:

- Back up your user presets!

- Program the desired version into an AM29F040B PLCC32 NOR Flash IC.
  These are widely available for as little as $1.

- With the power off, insert the programmed AM29F040B into U13, the
  (usually) empty PLCC32 socket at the top right of the Audity 2000 PCB.
  Pay very close attention to the chip orientation, and be careful with
  the insertion!

- Place a jumper across the two lower pins of W1, labelled "8"

- Power up the Audity 2000, and observe it booting from the upgrade ROM.

  Once booted, menu options available are:

  1.  Show current version
  2.  Show flash chip ID [*]
  3.  Install OS update
  4.  Dump OS to MIDI

  There is a video demo of the upgrade process at:

  https://www.youtube.com/watch?v=V7Mba2Qw8JA

- After updating, power off the Audity 2000, remove the jumper, and
  the upgrade ROM.

- At next power-on the NVRAM will be reset and the factory presets will
  be restored, and you should restore your user presets if desired.

[*] NB: this update ROM currently only supports Intel or Micron
    28F800 flash devices.   If your Audity has AMD flash memories
    instead please send me a photo of them along with the output
    of the "Show flash chip ID" screen.   Find me on Facebook in
    pretty much any E-mu group!
