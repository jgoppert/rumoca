# rumoca ![CI](https://github.com/github/jgoppert/rumoca/workflows/rust.yml/badge.svg)

A Modelica Compiler written in RUST.

## Building, Testing, and Running

```bash
cargo build
cargo run
cargo test
cargo run -- --filename src/model.mo --generator sympy
```

## Installing

```bash
cargo install --path .
```

Make sure you add your rust bin path to your .bashrc and source it, then:

```bash
$ rumoca --help
Modelica Compiler

Usage: rumoca [OPTIONS] --filename <FILENAME> --generator <GENERATOR>

Options:
  -f, --filename <FILENAME>    The filename to compile
  -v, --verbose                Verbose output
  -g, --generator <GENERATOR>  Generator to Use [possible values: sympy, json, casadi-mx, casadi-sx]
  -h, --help                   Print help
  -V, --version                Print version
```