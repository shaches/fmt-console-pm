# fmt Console App Template (PM Selectable)

This repository is a **Project Template** designed for use with the [cpp-hub](https://github.com/shaches/cpp-hub-demo) CLI tool.

It serves two purposes:
1.  **Practical:** Quickly scaffold a C++ console application that uses the modern `{fmt}` library.
2.  **Educational:** Demonstrate the advanced **"Overlays"** feature of `cpp-hub`, allowing a single template to radically change its file structure and build logic based on user input.

## Features

* **Modern C++:** Selectable C++ Standard (17, 20, or 23).
* **Dependency Management:** The user chooses how the `{fmt}` library is provided at generation time.
* **Zero-Overhead Option:** Can optionally generate a "vanilla" C++ project with *no* external dependencies.

## Usage

To generate a new project from this template using `cpp-hub`:

```bash
# If registered in your registry:
cpp-hub new fmt-console-pm

# Or directly from Git:
cpp-hub new --git https://github.com/shaches/fmt-console-pm.git
