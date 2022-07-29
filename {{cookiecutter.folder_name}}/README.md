![](https://img.shields.io/badge/code%20style-black-000000.svg)

# Development

## Install dev requirements
```shell
pip install -r requirements-dev.txt
```

## Install pre-commit
- add hooks
  ```shell
  pre-commit install
  pre-commit install --hook-type commit-msg
  ```
- update to the latest versions 
  ```shell
  pre-commit autoupdate
  ```

## Formatting and Linting
```shell
pre-commit run --all-files
```

## Run test
```shell
pytest --cov={{cookiecutter.module_name}} --cov-report html
```
