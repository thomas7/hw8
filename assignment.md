Write an Assignment

The objective of this assignment is to practice writing a bash script as well as to gain familiarity with regular expressions.

You are to write a bash script, average.sh, that reads in numbers from stdin until it is closed. You should take the average of these numbers and output it to a file given as an argument with the program.

Numbers may be entered into the command line as either integers or floats, if integers are used, than the average calculated should also be an integer. Likewise, if floats are used, the average should be a float. Floats should have a precision to the hundreths place (2 digits after the decimal). In order to check if the input is an integer or float, you MUST use regular expressions. Hint: Check out man pages for awk.

Standard error checking should be performed. Informative errors should be displayed to stderror for the following cases: 

+ The output file is not passed as an argument
+ Anything besides integers and floats are entered as input
+ Floats inputted do not have correct precision, i.e. 12.344 instead of 12.34

Example:  
$ ./average.sh output.txt  
1  
2  
3  
4  
^D  
In output.txt:  
10

Example 2:  
$ ./average.sh output2.txt  
1.10  
2.20  
3.30  
4.40  
^D  
In output2.txt:  
2.75

