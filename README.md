# Excel-Sheet
Program to generate excel sheet column sequence

Excel Sheet Column sequence means a sequence like A,B,C..Z,AA,AB..ZZ,AAA...ZZZ..... . The program is very simple to code once we understood the logic. For converting a number to the corresponding string in this sequence, we need to know two things : -

How many characters are there in the string.
What is the corresponding value of each character.
To find how many characters are there in the string, we should keep on diving the number/26 until it is greater than 0. To get the corresponding value of each character from last, we need to get number mod 26. One tricky thing about this algorithm is that, when we do the modulus of number corresponding to 'Z', we will get 26 mod 26 =0. We can add 26 to the modulus value if we get 0. Also in case of 'Z' , we need to subtract 1 from the result of number/26 so that our loop won't go for an extra iteration.

For generating the Excel Sheet Column sequence to a given number, convert all the numbers from 1 to given number to the corresponding sequence and put in a set and return it.
