# rpi-rp2-gcc

## Get the SDK and Examples

```shell-session
$ cd pico-volume-root
$ ./get-sdk-and-examples.sh
Cloning into 'pico-sdk'...
```

## Setup the Toolchain

```shell-session
$ docker-compose build pico
Building pico
...
Successfully tagged rpi-rp2-gcc_pico:latest
```

## Build the Examples

```shell-session
$ docker-compose run pico
# cd /root/pico/pico-examples
# mkdir -p build && cd $_
# cmake ..
# cd blink
# make -j4
```

Now you have blink.uf2 in `pico-examples/build/blink/`, and you can drag and drop it into RPI-RP2 to load it.

## References

- https://datasheets.raspberrypi.org/pico/getting-started-with-pico.pdf
