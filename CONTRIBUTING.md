# Contributing

## Getting Started

1. Fork the repository and clone it locally.
2. Create a virtual environment and install dependencies:
   ```bash
   python -m venv .venv
   source .venv/Scripts/activate  # Windows: .venv\Scripts\activate
   pip install -r requirements-dev.txt
   ```
3. Install the pre-commit hook:
   ```bash
   pre-commit install
   ```

## Making Changes

1. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
2. Make your changes in `src/`.
3. Add tests in `tests/`.
4. Run the linter and tests:
   ```bash
   ruff check .
   pytest
   ```
5. Commit and push your branch, then open a pull request against `master`.

## Code Style

- This project uses [ruff](https://docs.astral.sh/ruff/) for linting and formatting.
- The pre-commit hook will run ruff automatically on each commit.
- Keep line length to 88 characters.

## Running Tests

```bash
pytest
```

Coverage is reported automatically. Aim to keep coverage above 80%.
