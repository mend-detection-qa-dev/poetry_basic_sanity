# Test Case: Poetry Basic Sanity

## Package Manager
Poetry

## Python Version Detection
- **Source**: tool.poetry.dependencies.python
- **Expected Version**: ^3.9 (any 3.9.x or higher, below 4.0)

## Files Present
- pyproject.toml - Poetry manifest with python = "^3.9"
- poetry.lock - Poetry lock file

## Dependencies
- requests==2.31.0
- Django==2.2.0
- flask==2.2.5

## Test Purpose
**Basic sanity test for Poetry** - equivalent to uv_basic test case.
Validates basic Poetry project with standard dependencies.
No priority conflicts, straightforward version detection.

## Expected Behavior
- Tool detects Poetry as package manager (poetry.lock present)
- Reads python version from tool.poetry.dependencies.python
- Successfully installs dependencies with Python 3.9+
