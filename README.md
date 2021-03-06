# www.rust-lang.org
> the home of the rust website

![CI](https://github.com/rust-lang/www.rust-lang.org/workflows/CI/badge.svg)

## Development

### Running the app locally

1. This is a [Rocket](https://rocket.rs/) app, which means we use the `nightly` channel of Rust. We use a specific nightly version to ensure consistent builds locally and on the server, and the version is defined in the `rust-toolchain` file. [`rustup`](https://rustup.rs) will automatically download that nightly for you when you run a cargo command.
1. Install `cargo watch` by running `cargo install cargo-watch` in your terminal.
1. To build the app and run the server, run `cargo watch -x run` in your terminal.
1. Navigate to http://localhost:7878 in your browser. If you make any updates to the styles, or any other project files, `cargo watch` will automatically restart the server for you, all you have to do is refresh your browser to see your changes.

### Where to edit

- If you would like to edit styles, you should edit [`src/styles/app.scss`](src/styles/app.scss). 
- If you would like to update group data, you should edit the `yml` files in [`src/data/`](src/data/).
- If you would like to edit page content, you should edit the `hbs` files in [`templates`](templates).

### Contributing

Please read our [`CONTRIBUTING.md`](CONTRIBUTING.md) before submitting a PR!
