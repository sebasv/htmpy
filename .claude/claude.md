# Claude Development Guidelines

## Package Manager

Use `uv` as the package manager and to run Python code:

```bash
# Install dependencies
uv sync

# Run Python scripts
uv run python script.py

# Run modules
uv run python -m module_name
```

## Type Checking

Always verify changes with pyright before considering work complete:

```bash
uv run pyright luk
```

Fix all type errors before committing.

## Testing

Always add unit tests covering edge cases for new functionality:

```bash
# Run all tests
uv run pytest luk_tests
```

### Test Requirements

- Cover happy path and edge cases
- Test error conditions and exception handling
- Verify expected results are delivered
- Ensure all tests pass before considering work complete
