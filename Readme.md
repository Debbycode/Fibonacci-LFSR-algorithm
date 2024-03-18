## Author
[Your Name]

## Project Overview
This project implements a Linear Feedback Shift Register (LFSR) simulation using the Fibonacci LFSR algorithm. The simulation is implemented in C++ and includes the following components:

FibLFSR.hpp and FibLFSR.cpp: These files contain the declaration and implementation of the FibLFSR class, which represents the LFSR and provides methods for simulating one step and generating multiple bits.

main.cpp: This file contains a simple demonstration of using the FibLFSR class to simulate LFSR operations.

test.cpp: This file contains unit tests for the FibLFSR class using the Boost test framework.

Makefile: This file specifies the rules for compiling and building the project.

## Register Bit Representation
The register bits in the FibLFSR class are represented as a string of binary digits (0 or 1). The register is initialized with a seed string provided by the user, and the tap position is set to the index of the last bit in the seed string. This representation was choson for its simplicity and ease of manipulation of the register bits using string operations.

## Unit Tests
The test.cpp file contains two supplied unit tests and four additional unit tests to ensure the correctness of the FibLFSR class functionality::

testStepInstr: This test case checks the functionality of the step() method of the FibLFSR class by comparing the output of consecutive step() calls with the expected results.

testGenerateInstr: This test case validates the behavior of the generate() method of the FibLFSR class by comparing the generated bit sequence with the expected result.

testInitialSeed: Verifies if the initial seed of all zeroes generates the expected output.

testAllOnesSeed: Verifies if the initial seed of all ones generates the expected output.

testAllZeroesSeed: Verifies if stepping through the LFSR with an initial seed of all zeroes generates the expected output.

testMoreSteps: Verifies if generating a larger number of bits using the generate() method produces the expected output.

These tests cover various scenarios to ensure the robustness and correctness of the FibLFSR class.

## Additional Information
Compilation: To compile the project, use the provided Makefile by running the command "make". This will generate the PhotoMagic executable for running the demonstration and the test executable for running the unit tests.

Execution: After compilation, execute the PhotoMagic executable "./PhotoMagic" to run the demonstration, or execute the test executable "./test" to run the unit tests.

## Issues Encountered
Encountered challenge when running the "./test" command to run the unit test. Returns 'no such file or directory: ./test'

## Other Source Files
main.cpp: This file contains a simple demonstration of using the FibLFSR class to perform LFSR operations. It showcases how to create an instance of the FibLFSR class, perform one step of the LFSR operation, generate multiple bits, and print the current state of the LFSR register.

