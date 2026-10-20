# Buzzer 1.4.2

Sets BLE transmit power to the ESP32-S3 maximum of +20 dBm for advertising, scanning, and the default inherited by new connections and reconnects. Startup serial output reports whether the request succeeded and reads back the configured power levels.

Target: Adafruit Feather ESP32-S3 8 MB / no-PSRAM, hardware family 1. Retains the 1.4.1 battery improvements and existing OTA protocol.

Validation: PlatformIO release build succeeded; all 9 OTA package tests passed, including image integrity, embedded version, hardware compatibility, and partition checks. Physical readback, OTA installation, range, and battery-life testing remain pending.

Power specification: https://documentation.espressif.com/esp32_s3_datasheet_en.pdf
