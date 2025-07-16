# Core Folder in STM32 Project

The `Core` folder contains the main source code and essential components for the STM32 microcontroller project. This directory holds configuration files, application source code, and important support files for firmware development on STM32 platforms.

## Folder Structure

Typically, the `Core` folder includes the following components:

- **Inc/**: Contains header files (*.h) that define functions, variables, data structures, and macros used throughout the project.
- **Src/**: Contains source files (*.c) that implement functions and program logic.
- **startup/** (if present): Startup files for the microcontroller, including memory setup, interrupt vector table, etc.
- **main.c / main.h**: Main program files, representing the entry point of the firmware.
- **system_stm32xxx.c / .h**: System configuration files for clocks and core settings.
- **stm32xx_it.c / .h**: Interrupt handler files.
- **HAL/LL configuration files**: Files for hardware abstraction and peripheral configuration.

## Purpose

- Manages all core source code for the STM32 application.
- Separates declarations (Inc/) from implementations (Src/) for easier development and maintenance.
- Ensures modularity, scalability, and code reuse for other STM32 projects.

## Usage

1. **Add the `Core` folder to your workspace/project in STM32CubeIDE, Keil, IAR, etc.**
2. **Edit files in `Inc/` and `Src/` to develop your desired features.**
3. **Build and flash the program to the STM32 microcontroller.**

## Notes

- Avoid editing auto-generated files (by STM32CubeMX, STM32CubeIDE) unless necessary.
- Always back up your source code before making significant changes.

---
