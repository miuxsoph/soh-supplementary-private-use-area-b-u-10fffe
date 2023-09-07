# 􏿾
The programming language called 􏿾.

## How do you use it?
The program starts with a bit tape containing 50,000 zeroes.
Here are the different commands (all overwrite the current bit unless otherwise specified):
* `` (SOH) takes input from STDIN, overwriting the bits it needs, encoded as utf-8 if the current bit is 1, otherwise, encoded as latin-1. Remember to end the input stream with an EOF!
* `􏿾` (U+10FFFE) prints the bits in the output bit buffer, decoded as utf-8 if the current bit is 1, otherwise, encoded as latin-1. No overwriting occurs.
* `1` places a bit into the output bit buffer. No overwriting occurs.
* `0` pops a bit from the output bit buffer.
* `>` moves the bit tape cursor right. No overwriting occurs.
* `<` moves the bit tape cursor left. No overwriting occurs.
* `-` takes the inverse of the current bit.
* `?` does not execute the next character if the current bit is 1. No overwriting occurs.
* `A` takes the binary AND of the previous two bits.
* `O` takes the binary OR of the previous two bits.
* `N` takes the binary NAND of the previous two bits.
* `X` takes the binary XOR of the previous two bits.
* `|` goes back to the beginning of the program. No overwriting occurs.
