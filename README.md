# Ventoy Docker

Run [Ventoy](https://www.ventoy.net) in a Docker image. May be useful for some distributions that cannot directly run Ventoy natively, like NixOS.

## Notice

Build and run the docker image should be done in root user.

## Build Ventoy image

Run `./build/ventoy.sh`.

## Run Ventoy

Run `./bin/ventoy <device>`, where `<device>` is the device to install Ventoy, like `dev/sda`.

**Please make sure that the passed device is correct.**
