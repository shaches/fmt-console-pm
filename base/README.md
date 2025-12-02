# {{project_name}}

{{project_description}}

This project was generated from **fmt-console-pm-overlay** using **cpp-hub**.

It demonstrates selecting a **package manager for the `fmt` library** at generation time.

Chosen package manager: `{{package_manager}}` (this is just documentation; the code itself is not conditional).

---

## Requirements

- CMake ≥ 3.16
- A C++ compiler with C++{{cpp_standard}} support
- `fmt` installed / available according to your chosen package manager:

- `system`:
  - Install fmt via your OS package manager.
- `vcpkg`:
  - Use `vcpkg` and the generated `vcpkg.json` / `CMakePresets.json`.
- `conan`:
  - Use Conan and the generated `conanfile.txt`.

---

## Build (generic)

```bash
cmake -S . -B build
cmake --build build
./build/{{project_name}}

