# Project_16_bit_CPU

## Introduction

The project focuses on creating and integrating two main components: the control unit and the datapath. These units are merged to form a fully functional processor capable of executing a predefined set of instructions.

## Design

![Design](./assets/design.png)

Figure 1: Represents the design of the 16-bit CPU.

## Implementation

The project is implemented using the following steps:

![Implementation](./assets/implementation.png)

Figure 2: Represents the implementation steps.

### Controller Unit

The Controller unit includes:

- **Instruction Memory**: Holds CPU instructions.
- **Program Counter (PC)**: A counter that increments as long as the clear signal is active.
- **Instruction Register (IR)**: Stores the current instruction being executed.
- **State Machine**: Manages the sequence of operations based on the current state.

### Datapath

The Datapath contains:

- **Data Memory**: Holds data for operations.
- **Mux 2-to-1**: Decides output based on the ALU input or the read data.
- **Register File**: Stores instruction or address.
- **Arithmetic Logic Unit (ALU)**: Performs computations.

### Processor Integration

Integrates the control unit and datapath with appropriate connections to ensure functionality and performance.

## Test Procedures and Results

- **ControllerStateMachine_tb (FSM_tb)**: Validates the Finite State Machine's state transitions.
- **Controller_tb**: Tests the Controller module for proper initialization and state management.
- **Datapath_tb**: Assesses the datapath for correct ALU operations and data handling.
- **testProcessor**: Ensures the entire processor unit functions as expected.

## Project Build

![Build](./assets/projectbuild.png)

Firgure 3: Represents the project build process.

## Project RTL View

![RTL View](./assets/projectrtlview.png)

Figure 4: Represents the project RTL view.

## Conclusion

The project successfully integrates the control unit and datapath to create a fully functional 16-bit CPU capable of executing a set of instructions. The processor is tested for performance and functionality, ensuring it meets the project requirements.
