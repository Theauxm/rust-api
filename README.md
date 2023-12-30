# rust-api
Home Network API for various device communcation on a Raspberry Pi running Raspbian.

# Usage
There are currently 2 parts to the API. The first being a Wake on LAN magic packet for waking a device, and the other being a set of endpoints meant to serve as a way to interact with addressable LED lights (rpi-ws281x).

## Wake On LAN

The following is used for Wake On LAN. https://docs.rs/wake-on-lan/latest/wake_on_lan/

# Installation

## Rust

It is recommended to install Rust from the official website: https://www.rust-lang.org/tools/install

- You can install rust with the following shell command:
`curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`

NOTE: If you get the following error after attempting to run `rustc -v`:
`error: command failed: 'rustc': No such file or directory (os error 1)`

Run the following commands to install the correct version of Rust for RPi 3:
`rustup toolchain install stable-arm-unknown-linux-gnueabihf`
`rustup default stable-arm-unknown-linux-gnueabihf`


## RPi ws281x Rust

The following GitHub repo should be cloned/compiled/installed alongside this one (refer to this repo's `README`): https://github.com/rpi-ws281x/rpi-ws281x-rust.
