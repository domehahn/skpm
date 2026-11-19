# Contributing to skpm

Thank you for your interest in contributing to `skpm`! We welcome bug reports, feature proposals, and code contributions that align with our security and reliability standards.

## Development Setup

1. **Prerequisites**:
   - Go 1.23+ installed (`go version`)
   - Git 2.30+

2. **Clone and Build**:
   ```bash
   git clone https://github.com/domehahn/skpm.git
   cd skpm
   go test ./...
   ```

## Development Workflow

1. **Branching**: Create a feature or bugfix branch from `main`:
   ```bash
   git checkout -b feat/my-enhancement
   # or
   git checkout -b fix/issue-description
   ```

2. **Code Standards**:
   - Run `gofmt -s -w .` before committing.
   - Run `go test -v -race ./...` to ensure all tests pass cleanly with race detection.
   - Keep dependencies minimal; prefer the Go standard library or canonized ecosystem libraries (`sklib`).

3. **Commit Messages**: Follow Conventional Commits:
   - `feat: add new capability ...`
   - `fix: resolve boundary validation issue ...`
   - `docs: update API documentation ...`
   - `test: add unit coverage for edge case ...`

4. **Pull Requests**:
   - Open a PR against `main`.
   - Ensure all automated CI checks pass.
   - Include a concise summary of changes and reference any related issues.

## Reporting Security Issues

Please **do not** file public issues for suspected security vulnerabilities. Refer to [SECURITY.md](SECURITY.md) for confidential reporting instructions.
