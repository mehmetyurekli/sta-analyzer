lexical analyzer for a language called star.

1- Identifiers:
•	Maximum identifier size is 10 characters. If you use an identifier larger than that, the lexical analyzer issues an error message.
•	STAR is case sensitive and all the keywords are lower case. Identifiers can use both upper/lower case.
•	Identifiers start with an alphabetic character (a letter) and are composed of one or more letters/digits/_ (underscore)
•	Example Token: Identifier(my_var_1)

2- Integer constants:
•	Maximum integer size is 8 digits. If you use an integer value longer than that, the lexical analyzer issues an error message.
•	Negative values are not supported.
•	Example Token: IntConst(1290)


3- Operators:
•	Valid operators of the language are +,-,*,/
•	Example Token: Operator(+)


4- Brackets:
•	Brackets are used for creating blocks of code for the loops.
•	LeftCurlyBracket:  {      • RightCurlyBracket:  }
•	Example Token: LeftCurlyBracket


5- String constants:
•	String constants of STAR are delimited by double quotes (ASCII code 34)as in “this is a string“.
•	Maximum string constant size is 256 characters
•	String constants cannot contain the double quote character. when you reach one, the string terminates.
•	If a string constant cannot terminate before the file end, there should be a lexical error issued.
•	If a string constant exceeds 256 characters there should be a lexical error issued.
•	Example Token: String(“Hello world!“)


6- Keywords: (all are case sensitive)
•	Keywords are: int, text, is, loop, times, read, write, newLine
•	Example Token: Keyword(int)


7- End of line:  '.'
•	Period character '.' is used to mark the end of line.
•	Example Token: EndOfLine


8- Comma:
•	Comma ',' is used as a separator whenever multiple attributes are possible in any command. These include multiple declarations and write statements.


9- Comments: Anything between /* and */ is a comment.
•	If a comment fails to terminate before the file end, there should be a lexical error issued.
•	Comments are just like blank space and they create no tokens.
