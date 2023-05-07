Download Link: https://assignmentchef.com/product/solved-java-application-that-executes-recursive-methods
<br>
5/5 - (3 votes)

I.Java application that executes the following 5 recursive methods, each of which returns a value (do NOT use System.out.print() inside the method definitions), and prints that value in the main() method, where x is a positive integer on the commandline (1st argument), and s is a String on the commandline (2nd argument).



A.   Method 1: Return and print in main() x number of s (ssss…), in other words print the String s, x times.

B.    Method 2: Return and print in main() the first character in s, x number of times (ssss…), where “s” is the first letter in String “s”.

C.    Method 3: Return and print in main() each letter in s two times (s0s0s1s1s2s2s3s3…) where s0 is the first letter, s1 is the second letter, s2 is the third letter, etc.

D.   Method 4: Return and print in main() each letter in s three times backwards (sn-1sn-1sn-1sn-2sn-2sn-2sn-3sn-3sn-3sn-4sn-4sn-4…) where sn-1 is the last letter, sn-2 is the second to last letter, sn-3 is the third to last letter, etc.

E.    Method 5: Return and print in main() a String which counts down by 1 for x, and deletes one letter for each recursion for s, until x becomes 1, or until s has only 1 letter (x s, x-1 s1 letter deleted, x-2 s2 letters deleted, x-3 s3 letters deleted…)

II.            Use the commandline arguments to enter one positive integer (a number) as 1st argument, and a String (a word) as the 2nd argument.

.        see this webpage for instructions on commandline arguments.

A.   You need to convert the 1st commandline argument to an integer:Integer number = Integer.parseInt(args[0]);

B.    Note that “number” is the same as “x” in the above explanation.

C.    You need to store the 2nd commandline argument in a String variable:String word = args[1];

D.   Note that “word” is the same as “s” in the above explanation.

E.    You may find it useful to use more than one parameter for some of your methods.

III.            At the beginning of the main method, check to make sure that the user entered the correct input.

.        If exactly one (1) positive integer argument is not entered on the commandline, then display an error message and end the program.

A.   You also need to have a try-catch statement just in case a non-integer is inputted as a commandline argument.

IV.            Make sure your code follows the

V.            Java Coding standard, in particular the Java documentation (Javadoc) comments that go above each method.

VI.            Write your original comments every 3-5 lines of code.

Every method should be preceded with a descriptive comment using the “JavaDoc” notational convention.The comment should name the method, describe its purpose, comment all parameters, the return value, and any exceptions using JavaDoc keywords.

Detailed description line by line:Begins with a slash, followed by two asterisks (/**)One asterisk (*)One asterisk (*), followed by @param, followed by the name of the parameter, followed by a description of the parameter (Omit if there are no parameters. Use one line for each parameter, so two parameters will have two lines. 3 parameters will have 3 lines. Etc.)One asterisk (*), followed by return, followed by a description of the return variable (Omit if the return value is void.)One asterisk (*), followed by @exception, followed by the class of the exception, followed by a description of when the exception is thrown. Only checked exceptions are required to be listed. Unchecked exceptions are not required to be listed. Omit exceptions if there are no exceptions that are thrown. (In other words, if you catch the exception within the method, you do not need to list the exception.) Use one line for each exception, so two exceptions will have two lines. 3 exceptions will have 3 lines. Etc.Ends with one asterisk, followed by one slash (*/)Example

/**

* Prints a word, prints a number, and returns integer 1

*

* @param word any string of Class String

* @param number an integer of any value

* @return the integer 1

* @exception MyException if the word starts with the letter ‘z’

* @exception YourException if the number is a zero(0)

*/

public static int method1(String word, Integer number) throws MyException, YourException{

//code…

if(word.charAt(0) == ‘z’){

//thrown, but not caught in method, so put in JavaDocs above

throw new MyException();

}

if(number == 0){

//thrown, but not caught in method, so put in JavaDocs above

throw new YourException();

}

try{

int x = 5 / 0;

}

catch(ArithmeticException exception){

System.out.println(“ERROR: Division by zero! ” + exception);

}