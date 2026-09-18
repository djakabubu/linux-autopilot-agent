# Contributing to Linux Autopilot Agent

First off, thank you for considering contributing! 🎉

## Code of Conduct

Be respectful and constructive. Harassment, discrimination and toxic behavior
are not tolerated.

## How to contribute

### 1. Report bugs

Open an issue with:

- A clear, descriptive title.
- Steps to reproduce.
- Expected vs. actual behavior.
- Your environment (OS, Python version, model used).

### 2. Suggest features

Open an issue describing the feature, why it's useful, and how it should behave.

### 3. Submit code

1. Fork the repository.
2. Create a branch: `git checkout -b feature/my-feature`.
3. Make your changes.
4. Ensure the code still runs: `python3 -m py_compile linux_autopilot.py`.
5. Commit with a clear message.
6. Push and open a Pull Request.

## Development guidelines

- **Keep it dependency-free.** This project intentionally uses only the Python
  standard library. New features should not require external packages.
- **Keep it single-file.** The whole agent lives in `linux_autopilot.py`.
  Prefer adding to it over splitting into modules, unless the change is large.
- **Safety first.** Any change to the risk engine must be conservative: when in
  doubt, classify as `CAUTION` or `DANGEROUS`.
- **Comment generously.** This project values readable, well-commented code.
- **English only.** Code, comments, docs and commit messages are in English.

## Testing

There is no test suite yet. If you add logic, please include a short manual
test description in your PR. A proper test suite is a welcome contribution.

## License

By contributing, you agree that your contributions are licensed under the
[MIT License](LICENSE).