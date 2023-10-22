```
0-alias
Creates an alias with the name ls and value rm *.
alias ls="rm *"

1-hello_you
Prints "hello user", where user is the current Linux user.
echo "hello $USER"

2-path
Adds /action to the PATH. /action should be the last directory the shell looks into when looking for a program.
export PATH="$PATH:/action"

3-paths
Counts the number of directories in the PATH.
echo $PATH | tr ':' ' ' | wc -w

4-global_variables
Lists all global environment variables.
printenv

5-local_variables
Lists all local variables, environment variables, and functions.
set

6-create_local_variable
Creates a new local variable named BEST with the value School.
BEST="School"

7-create_global_variable
Creates a new global variable named BEST with the value School.
export BEST="School"

8-true_knowledge
Prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE.
echo $(($TRUEKNOWLEDGE+128))

9-divide_and_rule
Prints the result of POWER divided by DIVIDE. Both POWER and DIVIDE are environment variables.
echo $(($POWER/$DIVIDE))

10-love_exponent_breath
Displays the result of BREATH to the power LOVE. Both BREATH and LOVE are environment variables.
echo $(($BREATH**$LOVE))

11-binary_to_decimal
Converts a number from base 2 to base 10. The number in base 2 is stored in the environment variable BINARY.
echo $((2#$BINARY))

12-combinations
Prints all possible combinations of two lower-case letters, except oo. One combination per line and the output is alphabetically ordered.
printf "%s\n" {a..z}{a..z} | grep -v 'oo'

13-print_float
Prints a number with two decimal places. The number is stored in the environment variable NUM.
printf "%.2f\n" $NUM

14-decimal_to_hexadecimal
Converts a number from base 10 to base 16. The number in base 10 is stored in the environment variable DECIMAL.
printf "%x\n" $DECIMAL
```