# Fork of OpenZeppelin's e2e library

This is a temporary fork of [OpenZeppelin's e2e](https://github.com/OpenZeppelin/rust-contracts-stylus/tree/main/lib/e2e) library to implement e2e testing for Stylus contracts written using the [Stylus Rust SDK](https://github.com/OffchainLabs/stylus-sdk-rs).

## Usage

Add the following dependency to Cargo.toml to use `e2e`:

```toml
e2e = { git = "https://github.com/TucksonDev/e2e-lib.git" }
```

## Added content on the fork
- [shims.rs](./e2e/src/shims.rs) and [storage.rs](./e2e/src/storage.rs): to provide mocks of common host imports in Stylus `wasm` programs (copied from `motsu`)
- "Exposing added modules" and "Exposing modules used in e2e tests" blocks in [lib.rs](./e2e/src/lib.rs)
- "Extra dependencies for adding shims" block in [Cargo.toml](./e2e/Cargo.toml)