# prefect-azure

## Welcome!

prefect-azure is a collection of prebuilt Prefect tasks that can be used to quickly construct Prefect flows.

## Getting Started

### Python setup

Requires an installation of Python 3.7+

We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.

These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).

### Installation

Install `prefect-azure` with `pip`

```bash
pip install prefect-azure
```

### Write and run a flow

```python
from prefect import flow
from prefect_azure.tasks import (
    goodbye_prefect_azure,
    hello_prefect_azure,
)


@flow
def example_flow():
    hello_prefect_azure
    goodbye_prefect_azure

example_flow()
```

## Resources

If you encounter and bugs while using `prefect-azure`, feel free to open an issue in the [prefect-azure](https://github.com/PrefectHQ/prefect-azure) repository.

If you have any questions or issues while using `prefect-azure`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack)

## Development

If you'd like to install a version of `prefect-azure` for development, clone the repository and perform an editable install with `pip`:

```bash
git clone https://github.com/PrefectHQ/prefect-azure.git

cd prefect-azure/

pip install -e ".[dev]"

# Install linting pre-commit hooks
pre-commit install
```
