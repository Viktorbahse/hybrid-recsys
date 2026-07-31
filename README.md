#### **Подготовка и активация окружения**
```bash
    # setup uv environment
    command -v uv &> /dev/null || curl -LsSf https://astral.sh/uv/install.sh | sh

    # Create a .venv local virtual environment (if it doesn't exist)
    [ -d ".venv" ] || uv venv

    # install requirements + pre-commit hook
    make setup

    # activate environment
    source .venv/bin/activate
```


#### **Pre-commit check**

```bash
    make pre-commit-check
