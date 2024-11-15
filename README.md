# ICS3203-CAT2-Assembly-Mutei-Stephen-Solovea-150889

# Assembly Language Programs for Control, Array Manipulation, Modularization, and Simulation

This repository contains four Assembly programs created to showcase control flow, array operations, modular programming, and input/output simulation using port-based actions.

## Program Summaries

### 1. Number Classification Program
- **Description**: This program reads a number from user input, checks if the number is positive, negative, or zero, and then outputs the corresponding classification.
- **Highlights**: Uses both conditional and unconditional jumps for flexible program flow based on the user's input.

### 2. Array Reversal Program
- **Description**: This program takes an array of integers from the user, reverses the array in place, and outputs the result.
- **Highlights**: The reversal is done without extra memory, using index swapping within a loop to achieve the effect.

### 3. Factorial Calculation with a Subroutine
- **Description**: This modular program calculates the factorial of an input number by calling a subroutine and handling register values via the stack.
- **Highlights**: Demonstrates the use of the stack for register preservation in modular code, with results stored in a specific register for easy access.

### 4. Sensor-Based Simulation Program
- **Description**: Simulates reading a sensor value and controls a motor or an alarm based on predefined thresholds.
- **Highlights**: Uses specific memory locations to simulate hardware components and performs actions based on the simulated sensor input.

## Compiling and Running Instructions

1. **Compiler Requirements**: These programs are designed for NASM assembler.
2. **To Compile and Run**:
   - Use `nasm -f elf <filename>.asm -o <filename>.o` to compile each file.
   - Link with `ld -m elf_i386 <filename>.o -o <filename>`.
   - Run the executable with `./<filename>`.

## Observations and Challenges

- **Control Flow**: Achieving smooth branching using both conditional and unconditional jumps required precise planning of program flow.
- **Array Reversal**: In-place reversal without additional memory required meticulous index management.
- **Modular Programming**: Managing registers through the stack effectively ensured modular integrity and correct results.
- **Sensor Simulation**: Simulating sensor input and motor/alarm control presented unique challenges in mirroring real-world behavior using memory manipulation.
