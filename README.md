# Integer-To-Roman

Theory 

I -            1,
V  -           5,
X   -          10,
XL   -         40,
L     -        50,
XC     -       90,
C       -      100,
CD       -     400,
D         -    500,
CM         -   900,
M           -  1000.


2 is written as II in Roman numeral, just two one's added together. 12 is written as XII, which is simply X + II. The number 27 is written as XXVII, which is XX + V + II.

# Special Cases

I can be placed before V (5) and X (10) to make 4 and 9. 
X can be placed before L (50) and C (100) to make 40 and 90. 
C can be placed before D (500) and M (1000) to make 400 and 900.

Example - 

If Num = 1500 now if we devide Num / 1000 => 1500/1000 it will tell us how many (M) will be needed ex - 1500/1000 = 1.5 Round down to 1 so 1 - M if Num = 2500 then the Symbols will be MM. 
Then will will check for the next Symbol 500 and so on and so forth.
So for 1500 it will be 
1500/1000 = 1.5 = 1 - M
500/500 = 1 - C
Ans = MC


Here's a breakdown of how the code works:

1. A list symbolList is defined, which contains sublists of Roman numeral symbols and their corresponding decimal values. The symbols are arranged in descending order based on their decimal values. This is important for the conversion algorithm to work correctly.

2. The variable result is initialized as an empty string, which will store the final Roman numeral representation.

3. The code iterates through the symbolList in reverse order using a for loop. This allows the algorithm to start with the largest possible Roman numeral symbols and gradually build the representation.

4. Inside the loop, it checks if the given integer num divided by the current symbol's value (val) is greater than zero. This condition determines if the current symbol should be included in the Roman numeral representation.

5. If the condition in step 4 is true, it calculates the number of times the current symbol should be repeated by dividing num by val and assigns it to the variable count.

6. The current symbol is then repeated count times using string multiplication and concatenated with the result string.

7. Finally, the num value is updated by taking the remainder of num divided by val using the modulus operator. This ensures that any remaining value that hasn't been represented by the current symbol is considered in the next iterations.

8. After iterating through all the symbols in the symbolList, the final result string is returned, representing the Roman numeral equivalent of the input integer.
