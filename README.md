

# Blinky example in Rust on the Nucleo-STM32F413ZH board

Small project example to be used as template for embedded software in Rust on the Nucleo-STM32F413ZH board.

It is a modified version of the project https://github.com/aholzbaur/rust-stm32f4-disco-blinky.

The board: https://www.st.com/en/evaluation-tools/nucleo-f413zh.html

### Application
A timer interrupt is used to let the green, red and blue user leds blink.


### Rust
On windows 10 I :
* download and execute rustup-init.exe
* cargo install cargo-binutils
* rustup component add llvm-tools-preview
* cargo install cargo-generate
* rustup target add thumbv7em-none-eabihf
* cargo install cargo-flash

### Develop
build and flash:
* cargo build
* cargo flash --chip STM32F413ZHTx

See the [original project homepage](https://github.com/aholzbaur/rust-stm32f4-disco-blinky) for using openocd and gdb.
