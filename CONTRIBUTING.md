# Contributing to Agent Browser

First off, thank you for considering contributing! It's people like you that make Agent Browser a great tool.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Setup](#development-setup)
- [Styleguides](#styleguides)
- [Commit Messages](#commit-messages)
- [Pull Request Process](#pull-request-process)

## Code of Conduct

This project and everyone participating in it is governed by our commitment to provide a friendly, safe, and welcoming environment for all.

## Getting Started

- Fork the repository
- Clone your fork locally
- Create a new branch for your feature or fix
- Make your changes
- Push to your fork and submit a Pull Request

## How Can I Contribute?

### Reporting Bugs

Before creating a bug report, please check the [existing issues](../../issues) to see if the problem has already been reported. When you create a bug report, please include as many details as possible using our bug report template.

### Suggesting Enhancements

Enhancement suggestions are tracked as [GitHub issues](../../issues). When creating an enhancement suggestion, please include:

- A clear, descriptive title
- A detailed description of the proposed feature
- Explain why this enhancement would be useful
- List some examples of how it would be used

### Your First Code Contribution

Unsure where to begin contributing? You can start by looking for issues tagged with:

- `good first issue` — Issues which should only require a few lines of code
- `help wanted` — Issues that need extra attention

### Pull Requests

1. Fill in the required template
2. Include screenshots for UI changes
3. Follow the styleguides
4. Make sure all tests pass
5. Update documentation as needed

## Development Setup

### Prerequisites

- [Bun](https://bun.sh/) >= 1.0 (or Node.js >= 20)
- Git

### Installation

```bash
# Fork and clone the repository
git clone https://github.com/YOUR_USERNAME/Agent-browser.git
cd Agent-browser

# Install dependencies
bun install

# Start development server
bun dev
```

### Running Tests and Checks

```bash
# Type checking
bun typecheck

# Linting
bun lint

# Formatting
bun format

# Build (verifies production build)
bun build
```

## Styleguides

### TypeScript / React

- Use TypeScript for all new code
- Follow the existing file and folder structure
- Use functional components with hooks
- Prefer server components where possible (Next.js App Router)
- Use `cn()` utility for conditional class names

### Tailwind CSS

- Use Tailwind CSS utility classes
- Follow mobile-first responsive design
- Respect the dark mode variant (`dark:`)
- Use CSS variables for custom values

### Code Style

The project uses ESLint and Prettier for code formatting. Configuration files are included in the repository.

### Components

- Import components from `@/components/ui/`
- Use shadcn/ui components as the base
- Follow Radix UI patterns for accessibility (ARIA attributes, keyboard navigation)

## Commit Messages

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

| Type     | Description                       |
| -------- | --------------------------------- |
| `feat`   | A new feature                     |
| `fix`    | A bug fix                         |
| `docs`   | Documentation only changes        |
| `style`  | Code style changes (formatting)   |
| `refactor` | Code refactoring without behavior change |
| `perf`   | Performance improvements          |
| `test`   | Adding or updating tests          |
| `chore`  | Maintenance tasks, dependencies   |
| `ci`     | CI/CD configuration changes       |

Examples:

```
feat: add dark mode toggle
fix: resolve hydration mismatch in layout
docs: update installation guide
```

## Pull Request Process

1. **Branch naming**: Use descriptive branch names (e.g., `feat/dark-mode`, `fix/hydration-error`)
2. **PR Template**: Fill out the pull request template completely
3. **Review**: At least one maintainer approval is required
4. **CI Checks**: All automated checks must pass
5. **Merge**: Squash and merge is preferred

### PR Checklist

- [ ] Code follows the styleguides
- [ ] Self-review completed
- [ ] Changes are documented
- [ ] No new warnings or errors introduced
- [ ] All tests pass (`bun typecheck`, `bun lint`, `bun build`)

## Questions?

Feel free to open an issue with your question or reach out to the maintainers.

Thank you for contributing!
