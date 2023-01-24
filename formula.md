In this example, the function will first concatenate the values of cells A2 and B2 using the & operator. Then it will match the concatenated value with the concatenated values of columns A and B from sheet2. MATCH function will return the position of the matched value and INDEX function will return the value at the matched position of column C.

Both the formulas will work fine, it depends on the preference of the user which one they want to use.

=INDEX(Sheet2!C:C, MATCH(A2&B2, Sheet2!A:A&Sheet2!B:B, 0))
