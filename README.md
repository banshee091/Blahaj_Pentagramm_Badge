# Blahaj_Pentagramm_Badge

Firmware:

Build WLED (https://github.com/Aircoookie/WLED) using PlatformIO with the following Environment using the Buildflags for BME280 and PIR:

`[env:d1_mini]
...
build_flags = ${common.build_flags_esp8266} -D USERMOD_BME280 -D USERMOD_PIRSWITCH -D PIR_SENSOR_PIN=13
...
`
