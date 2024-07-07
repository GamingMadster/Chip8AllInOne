# Chip-8 All-In-One
This repo homes the All-In-One chip 8 test rom.

This test rom requires the following opcodes:

- All opcodes from the IBM-Logo test rom
- a semi-functional `FX0A` opcode (just pause execution until a key is released if you don't have this opcode implemented)

## Definitions:

✅ - Pass / Enabled   
❌ - Fail   
➖ - Disabled / Skipped

### 7XNN Test:
1 - Does the proper function   
2 - Is masked with 0xFF (or already wraps around when overflowed)

### 8XY0, 8XY1, 8XY2 Tests:
1 - Does the proper function   
2 - Quirk is enabled   
3 - vF is set in the proper order

### 8XY4, 8XY5, 8XY7 Tests:
1 - Does the proper function   
2 - Sets vF correctly on no overflow   
3 - Masks vX properly on overflow   
4 - Sets vF correctly on overflow   
5 - vF works as vX on no overflow   
6 - vF works as vX on overflow

### 8XY6, 8XYE Tests:
1 - Does the proper function   
2 - Quirk is enabled   
3 - vY stays unchanged   
4 - vF is set properly   
5 - vF can be used as vY (will show as - if quirk is enabled)   
6 - vF can be used as vX

## FX1E Tests: (Requires 55/65 to work properly)
1 - Does the proper function
2 - Doesn't change vF
3 - I is masked, or atleast handled as a u16 (Will fail in megachip)
