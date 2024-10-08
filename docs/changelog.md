## v1.6

No functional changes, just fixing the build after apparent toolchain updates on dev.

<3 @0xchocolate (cococode)


## v1.5

Fixes app to build with the new API. Thanks @Willy-JL for doing the hard part!


## v1.4

Turbo mode (gotta go fast)! The app now supports flashing as fast as possible (921600 baud with built-in retries). In my testing, this sped up a 1:37min flash to 23 seconds. Now we can't go back to the slow way!


## v1.3

No functionality changes. Fixed the build by removing deprecated API calls that weren't needed.


## v1.2

Firmware switching! The app now supports flashing two different firmware apps to slot A and slot B and uses the otadata partition (initialized by boot_app0) to switch between them. Make sure your firmwares are compiled to use the same partition table to avoid issues!


## v1.1

Auto-reset and notifications! For supported boards (RTS and DTR connected), flasher will now automatically enter the bootloader and reset the board. Also added notifications for user feedback (blue LED for duration of flash, vibrate when done).


## v1.0

Initial ESP flasher release! Supports hardcoded addresses for bootloader, partition table, NVS, boot_app0, and firmware, with a toggle for ESP32-S3 (different bootloader address).
