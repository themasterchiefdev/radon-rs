# Radon Rust

Python code metrics, implemented in Rust. Built in the open with **Harness**, Rajiv Yanamandra's software factory.

Radon Rust is a port of [Radon](https://github.com/rubik/radon). It will analyze Python source and report raw line metrics, cyclomatic complexity, Halstead metrics, and Maintainability Index.

**Status: project setup.** The analyzer is not implemented yet, and no installable release is available. Compatibility and performance claims will be backed by published tests and measurements as implementation progresses.

## Follow the build

- [Compatibility baseline](docs/compatibility.md): what the port intends to preserve.
- [Feature inventory](docs/features.csv): 102 upstream capabilities, with separate Rust implementation status.
- [Issues](https://github.com/themasterchiefdev/radon-rs/issues): report bugs, request features, or ask about the product.
- [Releases](https://github.com/themasterchiefdev/radon-rs/releases): verified builds when available.

The first implementation target is a bounded command that reads a Python file and reports raw metrics. Further work will add the remaining metrics, command options, and selected integrations. Scope decisions and verified behavior will be documented as they are made.

## Built with Harness

This project is a public demonstration of the software delivered with Harness. Follow product changes, tests, and releases to assess the results. Interested in using Harness for your own product? [Open a Harness enquiry](https://github.com/themasterchiefdev/radon-rs/issues/new?template=harness-enquiry.yml).

## Maintenance and license

Rajiv Yanamandra is the sole code contributor and maintainer. Bug reports and feature requests are welcome. External pull requests are not accepted; see [CONTRIBUTING.md](CONTRIBUTING.md). This intake policy does not limit your rights under the [MIT license](LICENSE).

Radon Rust is an independent port and is not affiliated with or endorsed by the upstream Radon maintainers. Retain upstream notices with any copied Radon code or fixtures.
