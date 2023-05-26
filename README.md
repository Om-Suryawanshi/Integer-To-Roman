# Integer-To-Roman

Theory 

Symbol       Value
I             1
V             5
X             10
XL            40
L             50
XC            90
C             100
CD            400
D             500
CM            900
M             1000


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
