# khyve

## How to build

```bash
sudo apt install gcc-riscv64-unknown-elf
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
rustup toolchain install nightly
rustup override set nightly
rustup component add rust-src
cargo install xargo
cargo install cargo-binutils
xargo build --target riscv64gc-unknown-linux-gnu
```
