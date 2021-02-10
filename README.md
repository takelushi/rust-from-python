# rust-from-python

Call Rust Program from Python.

## Commands

### Setup

```sh
# Setup Python.
poetry install
```
### Development

```sh
# Build Rust module.
poetry run maturin develop
# Run Python script.
poetry run python src/example/__init__.py
```

### Build

```sh
# Need to remove pyenv/shims PATH.
poetry run maturin build
# pyenv install 3.6.12
python -c 'from example import run;run()'
```

### Publish to PyPi

```sh
poetry run maturin publish
```

## Initialize Project

```sh
poetry init
cargo init --lib
```
