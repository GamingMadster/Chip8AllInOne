# Chip-8 All-In-One
This repo homes the Chip-8 All-In-One test ROM.

![Screenshot of the title page of the ROM captured in Octo.](Images/test_startup.png)

## Prerequisite
This ROM has been made to be run on STOCK Chip-8. While other variants of Chip-8 are recognized by the program through the usage of quirks, it is intended to debug stock Chip-8 interpreters.

### Required Opcodes
This ROM requires certain opcodes to allow general function of the tests. This includes:
- `1NNN`
- `6XNN`
- `ANNN`
- `DXYN`
- `FX0A`

## Opcode Tests
For more information on the details of how each test works, and their error codes, visit the [Test Documentation](Information/OpcodeTests.MD).

### Test Definitions
After running a test on an opcode, the test will return one of three possible outcomes.
- A tick mark, "✔": Test Passed
- A dash, "➖": Test Skipped
- A Number: Test Failed; different tests have a different number of error codes.

### Conditionals
- `3XNN`
- `4XNN`
- `5XY0`
- `9XY0`

### Subroutines
- `2NNN`
- `00EE`

### Arithmetic
- `8XY0`
- `8XY1`
- `8XY2`
- `8XY3`
- `8XY4`
- `8XY5`
- `8XY6`
- `8XY7`
- `8XYE`

### Memory
- `FX1E`
- `FX55`
- `FX65`

### Miscellaneous
- VIP Accuracy Test
