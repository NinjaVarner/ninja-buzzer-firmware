# Ninja Buzzer firmware 1.5.1

For the Feather ESP32-S3 8MB/no-PSRAM buzzer, hardware ID1, signed OTA protocol2.
Use Ninja Buzzer public Android app V3.10/code79 or newer.

Bluetooth updates verify a publisher signature and image compatibility/hash,
require physical authorization, and validate startup before accepting the new
image. Incomplete transfers preserve the previous bootable image; a failed new
startup rolls back. Real-board tests exercised rejection, abort, partial reset,
all-power-loss, startup-failure rollback and successful authenticated upgrades.

Authorize an update while idle: hold the large buzzer button, tap board RESET,
keep holding until the LED turns blue, then release. Use the app's Device
Information update controls and keep power connected through reboot and success.

Legacy protocol1 firmware requires a one-time supplier USB migration with a
verified recovery backup. It cannot become a secure updater merely by hiding
unsigned images in the Android interface. Do not attempt to install this file
through an old unsigned updater.

Image SHA256:
`53293bdfefbaab157fb9c8929c695b41a85107b2c32042a4af65cce2de3d2e24`

Publisher key ID:
`604ae11c91d278afb9f55b1dc9d5617fa5d38109a3461386a492cba9da7447ca`

The Raspberry Pi spectator is outside this release. No calibrated electrical
timing-accuracy or automated physical-endurance certification is claimed.
