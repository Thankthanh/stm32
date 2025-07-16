# Core Folder in STM32 Project

The `Core` folder contains the main source code and essential components for the STM32 microcontroller project. This directory holds configuration files, application source code, and important support files for firmware development on STM32 platforms.

## Folder Structure

Typically, the `Core` folder includes the following components:

- **Inc/**: Contains header files (`*.h`) that define functions, variables, data structures, and macros used throughout the project.
- **Src/**: Contains source files (`*.c`) that implement functions and program logic.
- **startup/** (if present): Startup files for the microcontroller, including memory setup, interrupt vector table, and low-level startup code.
- **main.c / main.h**: Main program files, representing the entry point of the firmware.
- **system_stm32xxx.c / .h**: System configuration files for clocks and core settings.
- **stm32xx_it.c / .h**: Interrupt handler files.
- **HAL/LL configuration files**: Files for hardware abstraction and peripheral configuration.
- **hethongnhung2.ioc**: STM32CubeMX project configuration file, which defines the hardware setup and auto-generates source files accordingly.

## Purpose

- Manages all core source code and configuration files for the STM32 application.
- Separates declarations (Inc/) from implementations (Src/) for easier development and maintenance.
- Ensures modularity, scalability, and code reuse for other STM32 projects.
- The `.ioc` file allows easy re-configuration and regeneration of code using STM32CubeMX.

## Usage

1. **Add the `Core` folder to your workspace/project in STM32CubeIDE, Keil, IAR, or other supported IDEs.**
2. **Edit files in `Inc/` and `Src/` to develop your desired features.**
3. **Use the `.ioc` file with STM32CubeMX to change hardware configuration or regenerate code as needed.**
4. **Build and flash the program to the STM32 microcontroller.**

## Notes

- Avoid editing auto-generated files (by STM32CubeMX, STM32CubeIDE) unless necessary, as changes may be overwritten when regenerating code from the `.ioc` file.
- Always back up your source code, especially before making significant changes or regenerating code.
- Keep the `.ioc` file under version control to track hardware configuration changes.
