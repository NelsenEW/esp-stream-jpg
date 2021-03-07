# Example esp_stream_jpg

Creates a http server and listen to `GET` requests at `http://[board-ip]/stream.jpg` with WIFI-STA mode. When the request is triggered, it streams QVGA JPEG image from the camera.

## Requirements

- ESP-IDF (V4.4)
- [esp32-camera](https://github.com/espressif/esp32-camera) repository as a submodule

## Instructions

1. Clone the repository including submodules

  ```
  git clone --recursive https://github.com/NelsenEW/esp_stream_jpg.git
  ```

2. Configure your WiFi SSID and Password via `idf.py menuconfig`


## Notes

* All camera pins are configured by default accordingly to A.I. Thinker and you can check then inside [Kconfig.projbuild](./main/Kconfig.projbuild).
* Make sure to read [sdkconfig.defaults](./sdkconfig.defaults) file to get a grasp of required configurations to enable `PSRAM` and set it to `64MBit`. PSRAM configuration should be added directly to `sdkconfig` once the `menuconfig` is done.

## TO-DO
* add AP-Mode capabilities (Currently, it only support STA mode).
