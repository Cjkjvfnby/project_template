![](https://img.shields.io/badge/code%20style-black-000000.svg)

# Development

## Install dev requirements
```shell
pip install -r requirements-dev.txt
```

## Formatting
```shell
black .
isort .
```

## Linting
```shell
flake8
```

## Run test
```shell
pytest --cov={{cookiecutter.module_name}} --cov-report html
```

## Install pre-commit
- install
  ```shell
  pip install pre-commit
  ```
- add hooks
  ```shell
  pre-commit install
  pre-commit install --hook-type commit-msg
  ```
- update to the latest versions 
  ```shell
  pre-commit autoupdate
  ```

Note:
flake8 dependencies are duplicated in the `additional_dependencies` section.
This might be a problem.
