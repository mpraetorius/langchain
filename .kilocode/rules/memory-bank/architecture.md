# Architecture

## System Architecture
The LangChain repository is structured as a monorepo, containing multiple independent packages within the `libs/` directory. This modular design allows for clear separation of concerns between the core logic (`libs/core`), community-contributed integrations (`libs/community`), and other specialized packages.

## Source Code Paths
- **Core Logic:** `libs/core/langchain_core/` - Contains the fundamental abstractions, interfaces, and runtime for the LangChain framework.
- **Community Integrations:** `libs/community/` - Houses the extensive collection of third-party integrations for LLMs, vector stores, document loaders, and more.
- **Documentation:** `docs/` - Contains all documentation, including API references, tutorials, and conceptual guides.
- **Command-Line Interface:** `libs/cli/` - Provides command-line tools for managing LangChain projects and integrations.

## Key Technical Decisions
- **Modularity:** The separation of `core` from `community` allows the core framework to remain lightweight and stable, while enabling rapid development and expansion of integrations.
- **Abstractions:** The use of base classes and abstract interfaces (e.g., `BaseLanguageModel`, `BaseRetriever`) is a core design principle, enabling a plug-and-play architecture.
- **Python-centric:** The primary implementation and focus of the repository is on the Python ecosystem.

## Component Relationships
- The `libs/core` package is the foundation upon which all other packages are built.
- `libs/community` depends on `libs/core` to implement the standard interfaces for its various integrations.
- The `docs/` are generated from the source code and narrative markdown files, providing a comprehensive guide to using the framework.
