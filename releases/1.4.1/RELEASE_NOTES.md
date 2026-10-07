# Buzzer 1.4.1

Reads the MAX17048 voltage and state-of-charge registers without resetting the gauge during detection. Adds a power startup delay, longer I2C timeout, and faster retries while readings are unavailable. Retains LC709203F support. Battery info now includes a sensor/startup status for app 2.34.

Target: existing Adafruit Feather ESP32-S3 8 MB / no-PSRAM hardware family 1. Hardware battery readings and OTA activation still need physical acceptance.

MAX17048 register conversion reference: https://www.analog.com/media/en/technical-documentation/data-sheets/MAX17048-MAX17049.pdf
