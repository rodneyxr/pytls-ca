# PyTLS-CA

PyTLS-CA is a Python application that quickly creates self-signed TLS certificates for your local development environment.

## Installation

This project uses [Poetry](https://python-poetry.org/) for dependency management. To install the project and its dependencies, run:

```sh
poetry install
```

## Usage

You can run the application with the following command:

```sh
poetry run pytls
```

You can specify options like the CA name, the services for which to generate certificates, and the output directory. For example:

```sh
poetry run pytls -n 'My Custom CA' -s service1 -s service2 -d './certificates'
```

## Options

- `-n`, `--ca-name`: The subject for the CA certificate. Defaults to `PyTLS CA`.
- `-s`, `--services`: The services for which to generate certificates. Can be specified multiple times for multiple services.
- `-d`, `--output-directory`: The directory in which to save the generated certificates. Defaults to `./certificates`.

## Development

This project uses [Ruff](https://docs.astral.sh/ruff/) for linting and code formatting.
