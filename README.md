# numberFormatterForCurrency

 JavaScript function that can convert a number to its equivalent value in thousands (K), millions (M), or trillions (T)

 This function takes in a number as an argument and returns a string that represents the number in either K, M, or T format. The toFixed method is used to format the number to one decimal place. The function works as follows:

If the number is greater than or equal to 1 trillion (10^12), it divides the number by 1 trillion and returns a string that represents the quotient with one decimal place followed by the letter 'T'.
If the number is greater than or equal to 1 billion (10^9) but less than 1 trillion, it divides the number by 1 billion and returns a string that represents the quotient with one decimal place followed by the letter 'B'.
If the number is greater than or equal to 1 million (10^6) but less than 1 billion, it divides the number by 1 million and returns a string that represents the quotient with one decimal place followed by the letter 'M'.
If the number is greater than or equal to 1 thousand (10^3) but less than 1 million, it divides the number by 1 thousand and returns a string that represents the quotient with one decimal place followed by the letter 'K'.
If the number is less than 1 thousand, it simply returns the original number as a string.
For example, if you call the function with the number 1234567890, it will return the string '1.2B'. If you call it with the number 9876543, it will return the string '9.9M'.