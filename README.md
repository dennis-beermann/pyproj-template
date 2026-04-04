# Python Project Template

A starter template for Python projects with a clean structure and common development tooling preconfigured. This includes

- Packaging (`pyproject.toml`)
- Dependency management
- Linting and formatting (`ruff`, `black`)
- Type checking (`mypy`)
- Testing (`pytest`, coverage)
- Pre-commit hooks
- CI workflow (GitHub Actions)
- Documentation scaffold
- Example `.env` and settings pattern

## TODO List (mention in this README)

- Python versions
    - in CI: see ci.yml
    - minimal version in pyproject.toml -> [project] -> requires-python
    - pyproject.toml -> tool.ruff -> target-version
- Project name currently "pyproj-template", rename accordingly in:
    - src/pyproj-template directory
    - pyproject.toml -> [project] -> name
- Define public API in src/pyproj-template/__init__.py
- line length for python files in
    - .vscode/settings.json -> [python] -> editor.rulers
    - pyproject.toml -> [tool.ruff] -> line-length
- License
    - pyproject.toml -> [project] -> license
- Pyright
    - Installed with "pip install -e ".[dev]". Alternatively install yourself to use from command line
    - Have pylance extension for VSCode installed, set it to use pyright
- Install uv (link to site) for dependency management. I installed it via PowerShell. Then run "uv sync" from repo root
- Install pre-commit via "uv run pre-commit install"
-
