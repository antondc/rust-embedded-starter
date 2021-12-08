# Leds

## Start OpenCD server

- Go to `/tmp` and use `openocd` to connect the device:

      cd /tmp
      openocd -f interface/stlink-v2-1.cfg -f target/stm32f3x.cfg

- On new tab start debug session with `cargo run` for this target:

      cargo run --target thumbv7em-none-eabihf -- -q -ex 'target remote :3333'
