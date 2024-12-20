# Contributing

We appreciate your interest in contributing. To ensure a smooth collaboration, please review the following guidelines.

> [!Note]
> Please ensure that your code passes all tests and `black` code formatting before opening a pull request.
> You can run the following commands to check your code:
> ```bash
> PYTHONPATH=src python -m unittest discover -s tests/ -p 'test*.py' -v
> black . --check
> ```

## How to Contribute

1. Get the latest version of the repository:
    - For the first time: Fork the repository. Clone the forked repository to your local machine.
    - For the second time: Sync your fork with the main repository.
2. Create a new branch for your changes:
    ```bash
    git checkout -b feature/new-feature
    ```
3. Make your changes and commit them:
    ```bash
    git commit -m "feat: add new feature"
    ```
4. Push your changes to your fork:
    ```bash
    git push origin feature/new-feature
    ```
5. Open a pull request to the main repository on the `main` branch.

## Code Style

- (Mandatory) Use [black](https://black.readthedocs.io/en/stable/) to format code
- Use [isort](https://pycqa.github.io/isort/) to reorder import statements
- Use [Google Docstring Format](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html) to standardize docstrings
- Use [Conventional Commits](https://www.conventionalcommits.org/) to make commit messages more readable
