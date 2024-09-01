# ${PROJECT_NAME} Repository

# Configure and Build

## Requirements

  - CMake 3.28+
  - Visual Studio 2022 or Visual Studio Code w/C++ Extension


## Configure Step

This is a very simple CMake template that is useful for quick and diryt
prototypes. For a complete project setup, see my cmake-cpp-template repository.

To configure the project:

```
cmake --preset=<preset_name>
```

The `<preset_name>` placeholder should be an available preset defined in
CMakePresets.json:

- windows-x86-debug
- windows-x86-release
- windows-x64-debug
- windows-x64-release
- linux-x86-debug
- linux-x86-release
- linux-x64-debug
- linux-x64-release

## Build Step

To build the project:

```
cmake --build --preset=<preset_name>
```

Alternatively you may open the project in Visual Studio or Visual Studio Code and
build from the menu after selecting your desire configuration. Other IDEs may
work, but they have not been tested.

By default, output binaries will be put into the project's `bin` directory. This
can be changed by setting the `${PROJECT_NAME_DEFINE}_OUTPUT_PATH` cache variable
in `CMakePResets.json`.
