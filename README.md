# Blahaj_Pentagramm_Badge

Firmware:

Build WLED (https://github.com/Aircoookie/WLED) using PlatformIO with the following Environment using the Buildflags for BME280 and PIR:

[env:d1_mini]
board = d1_mini
platform = ${common.platform_wled_default}
platform_packages = ${common.platform_packages}
upload_speed = 921600
board_build.ldscript = ${common.ldscript_4m1m}
build_unflags = ${common.build_unflags}
build_flags = ${common.build_flags_esp8266} -D USERMOD_BME280 -D USERMOD_PIRSWITCH -D PIR_SENSOR_PIN=13
lib_deps = ${esp8266.lib_deps}
monitor_filters = esp8266_exception_decoder
