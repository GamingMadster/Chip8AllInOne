# Opcode Test Documentation

## Conditionals
![Screenshot of the conditionals page of the ROM captured in Octo.](Images/conditionals.png)

`3xnn` - If register `x` is equal to `nn`, skip the next opcode.
`4xnn` - If register `x` is not equal to `nn`, skip the next opcode.
`5xy0` - If register `x` is equal to register `y`, skip the next opcode.
`9xy0` - If register `x` is not equal to register `y`, skip the next opcode.

### Failure Codes
`1` - Opcode always skips the next opcode.
