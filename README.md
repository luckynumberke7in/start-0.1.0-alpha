**NOTE:** This fork was created to update the cargo-leptos template to work with 0.1.0-alpha, and was merged into the main branch, but quickly became obsolete as cargo-leptos and leptos are changing very rapidly. I will hold off on updating this for now.

# Leptos Starter Template

This is a template for use with the [Leptos](https://github.com/gbj/leptos) web framework and the [cargo-leptos](https://github.com/akesson/cargo-leptos) tool.

## Creating your template repo

If you don't have `cargo-leptos` installed you can install it with

`cargo install --locked cargo-leptos`

Then run

`cargo leptos new --git https://github.com/leptos-rs/start`

to generate a new project template.

`cd {projectname}`

to go to your newly created project.

Of course you should explore around the project structure, but the best place to start with your application code is in `src/app/mod.rs`.

## Running your project

`cargo leptos watch`

## Installing Additional Tools

By default, `cargo-leptos` uses `nightly` Rust, `cargo-generate`, and `sass`. If you run into any trouble, you may need to install one or more of these tools.


1. `rustup toolchain install nightly --allow-downgrade` - make sure you have Rust nightly
2. `rustup default nightly` - setup nightly as default, or you can use rust-toolchain file later on
3. `rustup target add wasm32-unknown-unknown` - add the ability to compile Rust to WebAssembly
4. `cargo install cargo-generate` - install `cargo-generate` binary (should be installed automatically in future)
5. `npm install -g sass` - install `dart-sass` (should be optional in future
