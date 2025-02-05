# alu-shell

This repository contains a series of Bash scripts under the directory init_files_variables_and_expansions.
Each script is exactly two lines long, begins with "#!/bin/bash", ends with a newline,
and uses only allowed operations. No usage of &&, ||, ;, bc, sed, or awk is present.
All files are executable.

Scripts:
- 0-alias: Creates an alias ls="rm *".
- 1-hello_you: Prints "hello <user>".
- 2-path: Appends /action to the PATH.
- 3-paths: Counts directories in the PATH.
- 4-global_variables: Lists environment variables.
- 5-local_variables: Lists local and environment variables and functions.
- 6-create_local_variable: Creates local variable BEST=School.
- 7-create_global_variable: Creates global variable BEST=School.
- 8-true_knowledge: Prints 128 + TRUEKNOWLEDGE.
- 9-divide_and_rule: Prints POWER divided by DIVIDE.
- 10-love_exponent_breath: Prints BREATH raised to the power LOVE.
- 11-binary_to_decimal: Converts BINARY (base 2) to decimal.
- 12-combinations: Prints all two-letter combinations (except "oo").
- 13-print_float: Prints NUM with two decimals.
- 14-decimal_to_hexadecimal: Converts DECIMAL to hexadecimal.
- 15-rot13: Performs ROT13 encryption/decoding.
- 16-odd: Prints every other line from input.
- 17-water_and_stir: Prints expected output for WATER and STIR.
