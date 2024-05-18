Building the RP2040 device code should be the same as building any other Raspberry Pi PICO C SDK-based program, as described in [the Getting Started With Raspberry Pi Pico manual](https://datasheets.raspberrypi.com/pico/getting-started-with-pico.pdf?_gl=1*eciha9*_ga*MTk0OTYyMjEwNi4xNzE2MDA2NTk1*_ga_22FD70LWDS*MTcxNjAwNjk3NC4xLjAuMTcxNjAwNjk3NC4wLjAuMA..).

 1. Setup the PICO C SDK and go through the example builds using cmake and make to ensure that you can build Pico programs
 2. git clone this repo to <repo_dir>.
 3. cd <repo_dir>/sigrok-pico
 4. copy pico_sdk_import.cmake from your pico-sdk repo to <repo_dir>/sigrok_pico/pico_sdk_sigrok
 5. export PICO_SDK_PATH=<path_to_your_pico_sdk>
 6. cd <repo_dir>/sigrok-pico/pico_sdk_sigrok
 7. `cmake .`
 8. `make`

You should now have a `pico_sdk_sigrok.uf2` file in the directory
