# stm32f2
This crate provides an autogenerated API for access to STM32F2 peripherals.
The API is generated using [svd2rust] with patched svd files containing
extensive type-safe support. For more information please see the [main repo].

[svd2rust]: https://github.com/japaric/svd2rust
[main repo]: https://github.com/adamgreig/stm32-rs

## Usage
Each device supported by this crate is behind a feature gate so that you only
compile the device(s) you want. To use, in your Cargo.toml:

```toml
[dependencies.stm32f2]
version = "0.1.0"
features = ["stm32f215"]
```

Include the "rt" feature to bring in support for `cortex-m-rt` as well.

For details on the autogenerated API, please see:
https://docs.rs/svd2rust/0.8.1/svd2rust/#peripheral-api

## Supported Devices
STM32F215
STM32F217