# stringToInteger-leetcode
The algorithm for myAtoi follows these steps:

Read in and ignore any leading whitespace.
Check if the next character (if not already at the end of the string) is '-' or '+'. Read this character in if it is either. This determines if the final result is negative or positive, respectively. Assume the result is positive if neither is present.
Read in the next characters until the next non-digit character or the end of the input is reached. The rest of the string is ignored.
Convert these digits into an integer (e.g., "123" -> 123, "0032" -> 32). If no digits were read, then the integer is 0. Change the sign as necessary (from step 2).
If the integer is out of the 32-bit signed integer range [-2^31, 2^31 - 1], then clamp the integer so that it remains in the range. Specifically, integers less than -2^31 should be clamped to -2^31, and integers greater than 2^31 - 1 should be clamped to 2^31 - 1.
Return the integer as the final result.
