# ICS3203-CAT2-Assembly-Mutei-Stephen-Solovea-150889

# Assembly Language Programs

This repository contains several Assembly Language programs developed for various tasks, including control flow, array manipulation, subroutine usage, and port-based simulation.

## Programs Overview

### 1. Control Flow and Conditional Logic
- **Purpose:** Classifies a user-input number as “POSITIVE,” “NEGATIVE,” or “ZERO” using branching logic.
- **Key Features:** Uses both conditional and unconditional jumps to manage flow effectively.

### 2. Array Manipulation with Looping and Reversal
- **Purpose:** Reverses an array of integers in place without using additional memory.
- **Key Features:** Implements looping and direct memory access for in-place reversal.

### 3. Modular Program with Subroutines for Factorial Calculation
- **Purpose:** Calculates the factorial of a given number using a subroutine.
- **Key Features:** Demonstrates modular code, register handling, and stack usage to preserve register values.

### 4. Data Monitoring and Control Using Port-Based Simulation
- **Purpose:** Simulates a control program that reads a sensor value and activates motor and alarm based on water levels.
- **Key Features:** Uses specific memory locations or input ports to simulate sensor-based motor control and alarm triggering.

## Compiling and Running

1. **Assembly Compiler**: These programs are designed to be run on an x86 assembler (e.g., NASM).
2. **Steps**:
   - Compile using `nasm -f <output format> <filename>.asm -o <filename>.o`
   - Link with `ld -m <output format> <filename>.o -o <filename>`
   - Run using `./<filename>`

## Insights and Challenges

- **Control Flow and Conditional Logic:** Choosing the correct jump instructions for branching presented a challenge in ensuring the flow is both logical and minimal in instructions.
- **Array Manipulation:** Memory management directly in assembly, especially for reversing an array without additional memory, required careful indexing.
- **Modular Program:** Using the stack for register preservation was essential to maintaining program integrity, especially when calling subroutines.
- **Data Monitoring and Control:** Simulating real-world ports and sensor interactions was complex due to the constraints of assembly language.
