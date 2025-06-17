# Bazel Multi-Language Demo

This repository demonstrates a simple Bazel workspace combining several languages.

## Languages

- **C++**: `main/` contains a small library and application.
- **Python**: `main/main.py` is built as a `py_binary`.
- **Shell**: `scripts/hello.sh` is provided as a `sh_binary`.
- **JSON/CFG**: configuration files live in `data/`.

## Building

```bash
# Build the C++ binary
bazel build //main:main_cpp

# Run the Python program
bazel run //main:main_py

# Execute the shell script
bazel run //scripts:hello_script
```

Tests can be run with `bazel test //tests/...`.
