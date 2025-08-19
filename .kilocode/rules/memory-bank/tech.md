# Tech Stack

## Technologies Used
- **Primary Language:** Python (>=3.9)
- **Package Management:** PDM is used for dependency management and package building, as indicated by `pdm-backend` in `build-system.requires`. UV is also used for managing local package sources.
- **Linting and Formatting:** Ruff is used for linting and formatting, configured in the `[tool.ruff]` section of the `pyproject.toml` files.
- **Testing:** Pytest is the primary testing framework, with various plugins like `pytest-asyncio`, `pytest-mock`, and `pytest-watcher`.
- **Type Checking:** MyPy is used for static type checking.
- **Documentation:** Sphinx is used for generating documentation, with `myst-parser` for Markdown support.

## Development Setup
The project is a monorepo with multiple packages located in the `libs/` directory. Each package has its own `pyproject.toml` file, defining its specific dependencies and scripts. The top-level `pyproject.toml` file defines the dependencies for the entire monorepo.

## Technical Constraints
- The project requires Python 3.9 or higher.
- The project uses a strict set of linting and formatting rules, enforced by Ruff.
- The project uses a comprehensive testing suite, with both unit and integration tests.

## Dependencies
The project has a large number of dependencies, including:
- `langchain-core`: The core LangChain library.
- `langchain-community`: Community-contributed integrations.
- `langchain-experimental`: Experimental features.
- Various partner packages for integrations with services like OpenAI, Anthropic, Google Vertex AI, etc.

## Tool Usage Patterns
- **PDM:** Used for managing dependencies, running scripts, and building packages.
- **Ruff:** Used for linting and formatting the codebase.
- **Pytest:** Used for running the test suite.
- **MyPy:** Used for static type checking.
- **Sphinx:** Used for generating documentation.
