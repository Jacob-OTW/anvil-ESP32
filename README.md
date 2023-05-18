# Anvil ESP32 libraries for Micropython

This repository contains the modules required to run Anvil on an ESP32

## Security Note
In order for the connection to work,
I had to remove the keyword-arguments from the ``wrap_socket`` call
in ``async_websocket_client.py``, I'm not sure what effect this has on security.

## Setup
- Install [Micropython](https://micropython.org/download/esp32/) on your ESP32 (tested on v1.20.0)
, I used thonny to flash the .bin file and manage files.
- Clone the repository onto your local machine.
- Copy ``main.py``, ``boot.py``, and ``modules`` on the ESP32's file system.
- Add your Wi-Fi credentials in the ``boot.py`` file.
- Add your uplink key in ``main.py``
- Proceed as you would on a Pico W


See https://anvil.works/pico for more information