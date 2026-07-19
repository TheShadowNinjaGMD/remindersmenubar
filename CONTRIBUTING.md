# Contributing to RemindersMenubar

Thank you for your interest in contributing to **RemindersMenubar**! By contributing, you help make this native tool better for everyone.

As this project is distributed under the **GNU General Public License v3.0**, all contributions you submit will also be bound by its terms.

## Table of Contents

- [Reporting Bugs](#reporting-bugs)
- [Suggesting Enhancements](#suggesting-enhancements)
- [Development Setup](#development-setup)
- [Pull Request Process](#pull-request-process)
- [Coding Guidelines](#coding-guidelines)

## Reporting Bugs

If you find a bug or unexpected behavior:
1. Search the **Issues** tab to make sure it has not already been reported.
2. If it is a new issue, open a bug report.
3. Provide a clear description, your **macOS version**, steps to reproduce, and any relevant logs or error details.

## Suggesting Enhancements

Have an idea for a feature? We would love to hear it:
1. Check existing issues to see if the feature is already under discussion.
2. Open a new issue and clearly explain how the feature works and why it would benefit users.

## Development Setup

To start working on the source code:
1. Fork the repository on GitHub.
2. Clone your fork locally:
   ```bash
   git clone https://github.com
   ```
3. Open `RemindersMenubar.xcodeproj` inside Xcode.
4. Select your Mac as the active run destination, build, and run.

## Pull Request Process

1. Create a fresh branch off `main` for your modifications:
   ```bash
   git checkout -b feature/your-feature-name
   ```
2. Keep your changes tightly focused on resolving a single issue or introducing one cohesive feature.
3. Commit your progress using explicit, clear message descriptions.
4. Push your feature branch to your GitHub fork:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Submit a **Pull Request (PR)** against our `main` branch. 
6. Describe your changes clearly in the PR template, referencing any closed issue tracking ID.

## Coding Guidelines

* **Consistency**: Align your implementation style with the existing formatting guidelines of the project's codebase.
* **Testing**: Manually build and check your changes thoroughly inside macOS before shipping code.
* **Licensing**: Do not integrate external code dependencies unless they are natively compatible with the **GNU GPL v3.0** copyleft protections.
