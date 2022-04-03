# JAVA- Python Problem Series For Beginners
## I cover all type of problems of Java-Python from Basic to Pro Level.
# Writer Intro
## **[Subham Maity](https://github.com/Subham-Maity)** who is contributing on **Java** part
## **[Subhasish Negel](https://github.com/Subhasish-Negel)** who is contributing on **Python** part


**Welcome to this book on "Learning JAVA- Python Problem Series For Beginners".
I love Programming. One of the aims I had when I started ```CodeXam``` was to make learning programming easy.**

**At ```CodeXam```, we ask ourselves one question every day: "How do we create awesome learning experiences?"**

### Help us improve this guide - Fork, Pull Requests, Shares and Likes are recommended !

### [Raw Document](https://docs.google.com/document/d/1PzsEHJE54b2QDDNra34MY7-9XOabJOct7ffi0-ywiuk/edit?usp=sharing)
## Chapters
*******

### Problem List 
#### Operators
* [**1.Board Percentage Calculator :**](#1board-percentage-calculator-)
* [**2.Sum of three numbers :**](#2sum-of-three-numbers-)
* [**3.Calculate CGPA :**](#3calculate-cgpa-)
* [**5.Convert Kilometers to miles**](#5convert-kilometers-to-miles)
* [**7.Multiplication table, from any number to any number**](#7-multiplication-table-from-any-number-to-any-number)
* [**9.Comparison operators to find out whether a given number is greater than the user entered number or not.**](#9comparison-operators-to-find-out-whether-a-given-number-is-greater-than-the-user-entered-number-or-not)
* [**10.Write the following expression in a Java / Python / in your program**](#10-write-the-following-expression-in-a-java--python--in-your-program)
* [**11.(Java)What will be the result of the following expression**](#11javawhat-will-be-the-result-of-the-following-expression)

*****
#### String
* [**4.Asks the user to enter his/her name and greets them with “Hello , have a good day” text.**](#4asks-the-user-to-enter-hisher-name-and-greets-them-with-hello-name-have-a-good-day-text)
* [**12.Convert a string to lowercase.**](#12-convert-a-string-to-lowercase)
* [**13.Replace spaces with underscores.**](#13-replace-spaces-with-underscores)
* [**14.Fill in a letter template which looks like below:**](#14-fill-in-a-letter-template-which-looks-like-below)
* [**15.Detects double and triple spaces in a string.**](#15-detects-double-and-triple-spaces-in-a-string)
* [**16. Check if a String contains only whitespaces**](#16-check-if-a-string-contains-only-whitespaces)
* [**24.Type of website**](#24type-of-website)
* [**25.Email by deleting the part**](#25email-by-deleting-the-part)
*****
#### Checking Related Problems(If-Else)
* [**6.Detects whether a number entered by the user is an integer or not.**](#6-detects-whether-a-number-entered-by-the-user-is-an-integer-or-not)
* [**20.Prime or not (input from the user)**](#20prime-or-not-input-from-the-user)
* [**21.Pass or fail**](#21pass-or-fail)
* [**22.Calculate income tax**](#22calculate-income-tax)
* [**23.Leap year or not.**](#23leap-year-or-not)
*****
#### Type Casting
* [**8.(Type Casting) Encrypt a grade by adding a number to it. Decrypt it to show the correct grade.**](#8-type-casting-encrypt-a-grade-by-adding-a-number-to-it-decrypt-it-to-show-the-correct-grade)
*****
#### Escape sequence
* [**17.(Escape sequence) format the following sentence using escape sequence characters only**](#17escape-sequence-format-the-following-sentence-using-escape-sequence-characters-only)
*****
#### Case Switch 
* [**19.Print the name of the month.**](#19print-the-name-of-the-month)
* [**18.Make a Calculator.**](#18make-a-calculator)
*****
#### Loop
##### Pattern Problems
* [**1.(Solid Rectangle)**](#1solid-rectangle)

# 1.Board Percentage Calculator :

## Exercise 

Write a program to calculate the percentage of a given student in a board exam. His marks from 5 subjects must be taken as input from the keyboard. (Marks are out of 100)

## Approach:
```javascript
So here we did like this
Marks Percentage =
(What is the total number you got in the exam / The sum of the all subjects highest number ) X 100
```
## Solution

### Java : 

```java
import java.util.Scanner;
public class CodeXam { //our class is CodeXam
    public static void main(String[] args) {
        System.out.println("Enter The Maximum Marks Of One Subject (example: Physics 100) ");
        Scanner sc = new Scanner(System.in);
        float max= sc.nextFloat();
        max= max*5 ;
        System.out.println("Enter the number of your Subject 1 (Physics) : ");
        float a = sc.nextFloat();
        System.out.println("Enter the number of your Subject 2 (Math): ");
        float b = sc.nextFloat();
        System.out.println("Enter the number of your Subject 3 (Biology) : ");
        float c = sc.nextFloat();
        System.out.println("Enter the number of your Subject 4 (Chemistry) : ");
        float d = sc.nextFloat();
        System.out.println("Enter the number of your Subject 5 (Optional) : ");
        float e = sc.nextFloat();
        float total = a+b+c+d+e;
        System.out.println("Total marks: " + total);
        System.out.println("Percentage of your 5 Subject is: ");
        float Percentage = (total/max)*100;
        System.out.println("Marks Percentage= "+ Percentage);
    }
}

```


### Python : 

```python
maximum_numbers = int(input("Enter The Maximum Marks of One Subject (example: Physics 100) : "))
 
physics = int(input("Enter the number of your Subject 1 (Physics) : "))
 
math = int(input("Enter the number of your Subject 2 (Math) : "))
 
biology = int(input("Enter the number of your Subject 3 (Biology) : "))
 
chemistry = int(input("Enter the number of your Subject 4 (Chemistry) : "))
 
optional = int(input("Enter the number of your Subject 5 (Optional) : "))
 
 
total_marks = physics + math + biology + chemistry + optional
max_possible_marks = (maximum_numbers*5)
 
print("Total marks : ", total_marks)
print("Percentage of your 5 Subject is: ", (total_marks/max_possible_marks)*100)
 

```
# 2.Sum of three numbers :


## Exercise
Write a program to sum three numbers




## Approach:
```javascript
So here we did like this
Take the input of the first three numbers, then sum them all

```
## Solution

### Java :

```java

import java.util.Scanner;
public class CodeXam {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the first number ");
        int a = sc.nextInt();
        System.out.println("Enter the 2nd number ");
        int b = sc.nextInt();
        System.out.println("Enter the 3rd number ");
        int c = sc.nextInt();
        int sum = a + b + c;
        System.out.println("Sum of the three number is " + a + " + " + b + " + "+ c +  " = " + sum );

    }
}


```


### Python :

```python
first_num = int(input("Enter the 1st number : "))
second_num = int(input("Enter the 2nd number : "))
third_number = int(input("Enter the 3rd number : "))
 
sum_of_numbers = first_num+second_num+third_number
 
# Printing using Python String formatting ,also known as String  interpolation
print(f"Sum of three numbers is : {first_num} + {second_num} + {third_number} = {sum_of_numbers}")
  

 

```
# 3.Calculate CGPA :

## Exercise
Write a program to calculate CGPA using marks of three subjects (out of 100)



## Approach:
```javascript
So here we did like this
(What is the total number you got in the exam) / (total number of subject x 10) 

```
## Solution

### Java :

```java

import java.util.Scanner;
public class CodeXam {
    public static void main(String[] args) {
 
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the number of your Subject 1 (Physics) : ");
        float a = sc.nextFloat();
        System.out.println("Enter the number of your Subject 2 (Math): ");
        float b = sc.nextFloat();
        System.out.println("Enter the number of your Subject 3 (Biology) : ");
        float c = sc.nextFloat();
 
        float Total = a+b+c;
        System.out.println("Total marks: " + Total + " out of 300");
        System.out.println("CGPA of your 3 Subject is: ");
        float cGPA = (Total/30);
        System.out.println("Your CGPA is = "+ cGPA);
    }
}

```


### Python :

```python

 sub1 = int(input("Enter the number of your Subject 1 (Physics) : "))
sub2 = int(input("Enter the number of your Subject 2 (Math) : "))
sub3 = int(input("Enter the number of your Subject 3 (Biology) : "))
 
total = sub1+sub2+sub3
print("Total marks :", total, "out of 300")
print("Your CGPA is", total/30)

```


#  4.Asks the user to enter his/her name and greets them with “Hello ```<name>```, have a good day” text.


## Exercise

write a program that asks the user to enter his/her name and greets them with “Hello <name>, has a good day” text.

## Approach:
```javascript
So here we did like this
Take the name as an input 
and print Hello first with user input 
and concatenate with have a good day!

```
## Solution

### Java :

```java

import java.util.Scanner;
public class CodeXam {
   public static void main(String[] args) {
       System.out.println("What is your name");
       Scanner sc = new Scanner(System.in);
 
       String name = sc.next();
       System.out.println("Hello " + name + " have a good day!");
   }
}
 

```


### Python :

```python

 name = input("What's your name ? \n")
 
print(f"Hello {name}, have a great day !")
 



```
# 5.Convert Kilometers to miles


## Exercise
Write a  program to convert Kilometers to miles.


## Approach:
```javascript
So here we did like this
Take the km as an input and multiply with 0.621371
 miles = km*0.621371
 

```
## Solution

### Java :

```java
import java.util.Scanner;
public class CodeXam {
    public static void main(String[] args) {
        System.out.println("Enter the value in kilometers");
        Scanner sc = new Scanner(System.in);
        double km = sc.nextDouble();
        System.out.println();
        double miles = km*0.621371;
 
        System.out.println("The value in miles is  "  +  miles  +  "  miles");
    }
}


```


### Python :

```python

 value_in_km = int(input("Enter the value in kilometers: \n"))
 
km_to_miles = (value_in_km * 0.621371)
print("The value in miles is : \n", km_to_miles)




```
# 6. Detects whether a number entered by the user is an integer or not.


## Exercise

Write a  program to detect whether a string by the user is an integer(number) return true or if not return false.

## Approach:
```javascript
So here we did like this
For java : The hasNext() is a method of Java Scanner class which returns true if this scanner has another token in its input.
So here sc.hasNextInt()method returns true if the next set of characters in the input stream can be read in as an int. 
If they can't be read as an int, or they are too big for an int or if the end of the file has been reached, then it returns false. 
hasNextInt() itself does not consume any characters.
 
For Python : Python String isnumeric() method is a built-in method used for string handling. 
The isnumeric() method returns “True” if all characters in the string are numeric characters, Otherwise, It returns “False”
 
 

```
## Solution

### Java :

```java
import java.util.Scanner;
public class CodeXam {
    public static void main(String[] args) {
        System.out.println("Enter your number");
        Scanner sc = new Scanner(System.in);
        System.out.println(sc.hasNextInt());
    }
}


```


### Python :

```python
user_input = input("Enter your number ")
 
print(user_input.isnumeric())
 

 

```
# 7. Multiplication table, from any number to any number

## Exercise

printing multiplication table for any number, from any number to any number (all given in input) (Forward and reverse order multiplication should be implemented in the program)

## Approach:
```javascript
So here we did like this
 
Forward : Run a incrementing for loop from Start to end and print the value of the given number what you want 
to get a multiplication table (note: Start < End ) 
Reverse : Run a decrementing for loop from Start to end and print the value of the given number what you want 
to get a multiplication table
(note: Start > End ) 
```
## Solution

### Java :

```java
import java.util.Scanner;
public class CodeXam
{
    public static void main(String[] args)
    {
        Scanner s = new Scanner(System.in);
        System.out.print(" Enter the number you want to get a multiplication table of : ");
        int n=s.nextInt();
        System.out.print("From where : ");
        int start=s.nextInt();
        System.out.print("To where : ");
        int end=s.nextInt();
 
        if (start <= end )
        for(int i=start; i <= end; i++)
        {
            System.out.println(n+" * "+i+" = "+n*i);
        }
        else{
            for(int i=start; i >=  end; i--){
                System.out.println(n+" * "+i+" = "+n*i);
            }
 
        }
    }
}


```


### Python :

```python

 value = int(input("Enter the number you want to get a multiplication table of : "))
start = int(input("From where : "))
end = int(input("To where : "))
 
 
if start <= end:
    for i in range(start, end+1):
        print(f"{value} * {i} = {value * i}")
elif start > end:
    for o in range(start, end-1, -1):
        print(f"{value} * {o} = {value * o}")


```
# 8. (Type Casting) Encrypt a grade by adding a number to it. Decrypt it to show the correct grade.

## Exercise
Write a program to the first user input his/her exam grade. Now the program asks for a code number to encrypt your grade by adding the number with your grade. Now the program asks you if you want to decrypt your grade press y or if no type n (note: Y/y or N/n case must be ignored and user can type the capital letter or small letter your program should understand)and if yes program will start decrypting your grade and show you your original grade otherwise program will print “ sorry sir/mam, we can't crack your grade “


## Approach:
```javascript
So here we did like this
Java: 1. First take a input as a char (letter like : A B C D ) 
      2. Take a input as an integer value 
      3. Type cast them because if we do any operation between char and int, it returns int (it’s called numaric Promotion Rules 
1.Byte + Short = Int  
2.Short + Int  = Int
3.Long + Float = Float
4.Character + Int = Int (here we use this)
5.Character + Short = Int
6.Long + Double = Double
7.Float + Double = Double)So we must have to cast them into char 
      4.Take a input as a string value (yes for y No for n) 
      6.we check the input letter(y/n) and also ignore case by equalsIgnoreCase 
      7.Type cast again and do this : Your given grade - Your given number 
 
==========================================================================
 
Python : To install “Click” package simply go to any terminal and type “pip install click”
 
1. We used 'Click' module by this command "import click"
2. Take a input as a string for your grade
3. Take a input as an string for your code
4. use 'click' for take yes or no on input
       
Python click module is used to create command-line (CLI) applications.
It is an easy-to-use alternative to the standard optparse and argparse modules.
 

```
## Solution

### Java :

```java
import java.util.Scanner;
public class CodeXam {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        System.out.println(" Enter Your Exam Grade ");
        char grade = sc.next().charAt(0);
        System.out.println("Enter Your Code Number We Will Encrypt Your Grade ");
        int a = sc.nextInt();

        // Encrypting the grade
        grade = (char)(grade + a);
        System.out.println("So Now Your Grade is : " + grade);

        // Ask User
        System.out.println("Sir/Mam, Do you want to decrypt your grade? If yes type " + " y/Y " + " If no type " + " n/N ") ;
        String answer = sc.next();

        // Decrypting the grade
        if ( (answer.equalsIgnoreCase("Y") ) ) {
            grade = (char) (grade - a);
            System.out.println("Your actual Grade is " + grade);
        }
        else
        {
            System.out.println("sorry Sir/mam, we can't crack your grade");
        }

    }
}


```


### Python :

```python

 import click
 
result = input("Please Enter Your Exam Grade: ")
code = input("Please Enter Your Encryption Code: ")
 
print("\nNow Your Grade is 'F'")
 
if click.confirm("\nSir/Ma'am, Do You Want to Decrypt Your Grade ? If Yes type 'Y/y' or 'N/n' for No :\n>> ",
                 default=True):
    print("Your Actual Grade is ", result)
else:
    print("Grade Decryption Aborted")

```
# 9.Comparison operators to find out whether a given number is greater than the user entered number or not.


## Exercise
Use comparison operators to find out whether a given number 28/56 is greater than the user entered number or not.



## Approach:
```javascript
So here we did like this
 
Take a number from the user and compare them using < / > and store it in the boolean data type because 
if you compare two operators it returns true or false

```
## Solution

### Java :

```java
import java.util.Scanner;
public class CodeXam {
    public static void main(String[] args) {
 
        Scanner ab = new Scanner(System.in);
        int a1 = 28;
        System.out.println("Given number is " + a1);
 
        System.out.println("Enter number = ");
 
        int a = ab.nextInt();
        System.out.println(a);
        boolean bool = (a1 >= a);
        if (bool){
            System.out.println("given number 28 is greater than your entered number ");
        }
        else {
            System.out.println("given number 28 is less than your entered number ");
        }
    }
}


```


### Python :

```python
given_number = 56
print("The given number is", given_number)
 
user_input = int(input("Enter your number : \n"))
 
if user_input < given_number:
    print("Given number is greater than the entered number")
elif user_input == given_number:
    print("Both are same number")
else:
    print("Given number", given_number, "is less than the entered number")
 

```
# 10. Write the following expression in a Java / Python / in your program

## Exercise
Write the following expression in a Java / Python / in your program
**(v^2-u^2)/2as**
<p align="center">
        <img src="https://github.com/Subham-Maity/java_python_problem_solving-series/blob/master/Image(ignore)/10.png?raw=true"/>
        </p>


## Approach:
```javascript
So here we did like this
Just do this
(v*v) - (u*u))/ (2*a*s)
```
## Solution

### Java :

```java
 
import java.util.Scanner;
 
public class CodeXam {
    public static void main(String[] args) {
        double v,u,a,s;
 
        Scanner sc = new Scanner(System.in);
        System.out.println("Equation is (v^2 -u^2)/(2as)");
        System.out.println("Enter your value of v");
        v = sc.nextInt();
        System.out.println("Enter your value of u");
        u = sc.nextInt();
        System.out.println("Enter your value of a");
        a = sc.nextInt();
        System.out.println("Enter your value of s");
        s = sc.nextInt();
 
        double d = ((v*v) - (u*u))/ (2*a*s) ;
        System.out.println("your result is "+d);
 
    }}


```


### Python :

```python

 print("\nEquation is (v^2 -u^2)/(2as)")
 
v = int(input("\nEnter the value of v: "))
u = int(input("Enter the value of u: "))
a = int(input("Enter the value of a: "))
s = int(input("Enter the value of s: "))
 
result = ((v*v) - (u*u))/ (2*a*s)
print("Your result is :", result)

```
# 11.(Java)What will be the result of the following expression

## Exercise
Why does this happen?
<p align="center">
        <img src="https://github.com/Subham-Maity/java-python-problem-solving-series/blob/master/Image(ignore)/11.png?raw=true"/>
        </p>




## Approach:
```javascript
So here we did like this for result we need to define the floating point
7/4 it always return an integer so 7/4 = 1 
                                Then 9/2 = 4
                                Then 1*4 = 4 (this is the reason why then 
 Our program return 4 instead of 7.875) 
```

# 12. Convert a string to lowercase.


## Exercise
Write a program to convert a string to lowercase. This string is given by the user.



## Approach:
```javascript
So here we did like this
Java : in java The toLowerCase() method converts a string to lower case letters
Python : in Python, the “ .lower” method is used to convert a string in lower case !
```
## Solution

### Java :

```java
import java.util.Scanner;
public class CodeXam {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter any sentence or word: ");
        String string = sc.nextLine();
        string = string.toLowerCase();
        System.out.println("In lower case this word or sentence looks like this : " + "\n" + string);
    }
}


```


### Python :

```python
given_str = input("Enter any sentence or word : ")
 
print("In lower case this word or sentence looks like this :", given_str.lower())

 

```
# 13. Replace spaces with underscores.

## Exercise

Write a program to replace spaces with underscores. This string is given by the user.

## Approach:
```javascript

So here we did like this
Java : The replace() method searches a string for a specified character, and
returns a new string where the specified character(s) are replaced.
Python : It's the same as Java, just use the .replace method.
```
## Solution

### Java :

```java
import java.util.Scanner;
public class CodeXam {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter any sentence with space: ");
        String string = sc.nextLine();
        string = string.replace(" ", "_");
        System.out.println("This sentence with underscores looks like this : " + "\n" + string);}}


```


### Python :

```python
txt = input("Enter your sentence with space : \n")
 
x = txt.replace(" ", "_")
 
print("This sentence with underscores looks like this:\n",x)


 

```
# 14. Fill in a letter template which looks like below:

## Exercise
Write a program to fill in a letter template which looks like below:
```javascript
Sentence =      “Dear <|name|>, Thanks a lot” 
 
Replace =      <|name|> with a string (some name)

```

## Approach:
```javascript
So here we did like this
Java : We use replace method but if we just do like this 
        String sentences = sc.nextLine();
        String sentence = "Dear <|name|>, Thanks a lot!";
        sentence.replace("<|name|>", sentences);
        System.out.println(sentence);
 It will execute this : Enter your name: Subham
                        Dear <|name|>, Thanks a lot!
If we want to change a string we need convert a string by storing it in 
another string variable
 
Python : We will use the .replace() method again and unlike java , we don’t need to store the string in another variable !


```
## Solution

### Java :

```java
import java.util.Scanner;
public class CodeXam {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter your name: ");
        String sentences = sc.nextLine();
        String sentence = "Dear <|name|>, Thanks a lot!";
        sentence =  sentence.replace("<|name|>", sentences);
        System.out.println(sentence);
    }
}



```


### Python :

```python
name = input("Enter your name: ")
 
output = "Dear <|Name|>, Thanks a Lot !"
 
print(output.replace('<|Name|>', name))
```

# 15. Detects double and triple spaces in a string.

## Exercise
Write a  program to detect the index of double and triple spaces in a string given by the user.
<p align="center">
        <img src="https://github.com/Subham-Maity/java-python-problem-solving-series/blob/master/Image(ignore)/15.png?raw=true"/>
        </p>

## Approach:
```javascript
So here we did like this
Java: The indexOf() method returns the position of the first occurrence 
of specified character(s) in a string
 
Python : The .index() method return the position of first occurrence 
of specified character(s) in a string

```
## Solution

### Java :

```java
import java.util.*;
public class code_xam {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter your Sentence ");
        String str1 = sc.nextLine();
        System.out.println(str1.indexOf("  "));
        System.out.println(str1.indexOf("   "));
    }
}



```


### Python :

```python
txt = input("Enter Your sentence with 2 and 3 spaces:\n")
print(txt.index("  "))
print(txt.index("   "))

```
# 16. Check if a String contains only whitespaces

## Exercise
Check if a String given by the user contains only whitespaces or not if the string has only whitespace print 
“ It is only whitespace” if not print “It’s a sentence ”

## Approach:
```javascript
So here we did like this
Java:
 
The Java String class trim() method eliminates leading and trailing spaces
he Java String class isEmpty() method checks if the input string is empty or not
 
Get the String to be checked in str1
We can use the trim() method of String class to remove the leading whitespaces in the string.
Syntax:
str1.trim()
Then we can use the isEmpty() method of String class to check if the resultant string is empty or not. If the string contained only whitespaces, then this method will return true
Syntax:
str.isEmpty()
Combine the use of both methods using Method Chaining.
str.trim().isEmpty()
Print true if the above condition is true. Else print false.
 
Python : We’re simply using if, else conditions here ! 


```
## Solution

### Java :

```java
import java.util.*;
class CodeXam {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter your Sentence");
        String str1 = sc.nextLine();
        {
            if (str1.trim().isEmpty())
                System.out.println("It is only whitespace");
            else
                System.out.println("It's a sentence");
        }}}



```


### Python :

```python
input_str = input("Please enter your sentence : \n")
 
if  input_str:
    print("It's a sentence")
else:
    print("It's only Whitespace")

```

# 17.(Escape sequence) format the following sentence using escape sequence characters only

## Exercise
format the following sentence using escape sequence characters only
<p align="center">
        <img src="https://github.com/Subham-Maity/java-python-problem-solving-series/blob/master/Image(ignore)/17.png?raw=true"/>
        </p>

## Approach:
```javascript
So here we did like this
Java :
Escape Sequence :
 
\t  Inserts a tab in the text at this point.
\b  Inserts a backspace in the text at this point.
\n  Inserts a newline in the text at this point.
\r  Inserts a carriage return in the text at this point.
\f  Inserts a form feed in the text at this point.
\'  Inserts a single quote character in the text at this point.
\"  Inserts a double quote character in the text at this point.
\\  Inserts a backslash character in the text at this point.
 
Python :
 
\'	Single Quote
\”    Double Quote	
\\	Backslash	
\n	New Line	
\r	Carriage Return	
\t	Tab	
\b	Backspace	
\f	Form Feed	
\ooo	Octal value	
\xhh	Hex value


```
## Solution

### Java :

```java
 
class CodeXam {
    public static void main(String[] args) {
        String myLetter = "Dear Xam,\n\tThis question answer sheet is very helpful for me .\n Thanks!";
        System.out.println(myLetter);
    }
     }



```


### Python :

```python
output = "Dear Suvo,\n\tThis question answer sheet is very helpful for me.\n Thanks!"
 
print(output)
```

# 18.Make a Calculator.

## Exercise
Make a Calculator. Take 2 integer numbers (a & b) from the user and an operation as follows
```javascript
Press 1 : + (Addition) a + b 
Press 2 : - (Subtraction) a - b 
Press 3 : * (Multiplication) a * b 
Press 4 : / (Division) a / b 
Press 5 : % (Modulo or remainder) a % b 
Calculate the result according to the operation given and display it to the user

```

## Approach:
```javascript
So here we did like this
Java : using case switch and take the integer input from the user and operation to them as 
the instructions are given in the question 
 
Python : We take all int value as input and simply use if elif method


```
## Solution

### Java :

```java
import java.util.*;
 
public class CodeXam {
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter Your First Number");
        int a = sc.nextInt();
        System.out.println("Enter Your Second Number");
        int b = sc.nextInt();
        System.out.println("Press 1 : + (Addition):  " +  a + " + " + b + "\nPress 2 :  - (Subtraction):  " +  a + " - " + b + "\nPress 3 :  * (Multiplication):  " +  a + " * " + b +"\nPress 4 :   / (Division):  " +  a + " / " + b +"\nPress 5 :  % (Modulo or remainder):  " +  a + " % " + b );
 
        int operator = sc.nextInt();
 
          /**
         * 1 -> +
         * 2 -> -
         * 3 -> *
         * 4 -> /
         * 5 -> %
           */
 
        switch(operator) {
            case 1 : System.out.println(a+b);
                break;
            case 2 : System.out.println(a-b);
                break;
            case 3 : System.out.println(a*b);
                break;
            case 4 : if(b == 0) {
                System.out.println("Invalid Division");
            } else {
                System.out.println(a/b);
            }
                break;
            case 5 : if(b == 0) {
                System.out.println("Invalid Division");
            } else {
                System.out.println(a%b);
            }
                break;
            default : System.out.println("Invalid Operator");
        }
    }
}




```


### Python :

```python
a = int(input("Enter your 1st number: "))
b = int(input("Enter your 2nd number: "))
 
print(f"""
Press 1 : + (Addition): {a} + {b}
Press 2 :  - (Subtraction): {a} - {b}
Press 3 :  * (Multiplication): {a} * {b}
Press 4 :   / (Division): {a} / {b}
Press 5 :  % (Modulo or remainder): {a} % {b}""")
 
user_input = int(input())
 
if user_input == 1:
    print(a+b)
elif user_input == 2:
    print(a-b)
elif user_input == 3:
    print(a*b)
elif user_input == 4:
    print(a / b)
elif user_input == 5:
    print(a % b)
else:
    print("Invalid Input :(") 

```

# 19.Print the name of the month.


## Exercise
Ask the user to enter the number of the month & print the name of the month. For eg - For ‘1’ print ‘January’, ‘2’ print ‘February’ & so on


## Approach:
```javascript
So here we did like this
Java : using case switch and take the integer input from the user and print according to the number
Python:Same as Java, we’re using Case switch method here, “match-case”.Python 3.10 (2021) introduced the
match-case statement which provides a first-class implementation of a "switch" for Python.

```
## Solution

### Java :

```java
import java.util.*;
 
public class CodeXam {
    public static void main(String args[]) {
        Scanner sc = new Scanner(System.in);
 
        System.out.println("Enter the number of the month \n(Press : 1 -12 only) " );
 
        int operator = sc.nextInt();
        String sentence = "The name of the month according to your number is: ";
 
        switch(operator) {
            case 1 : System.out.println(sentence + "January");
                break;
            case 2 : System.out.println(sentence + "February");
                break;
            case 3 : System.out.println(sentence + "March");
                break;
            case 4 : System.out.println(sentence + "April");
                break;
            case 5 : System.out.println(sentence + "May");
                break;
            case 6 : System.out.println(sentence + "June");
                break;
            case 7 : System.out.println(sentence + "July");
                break;
            case 8 : System.out.println(sentence + "August");
                break;
            case 9 : System.out.println(sentence + "September");
                break;
            case 10 : System.out.println(sentence + "October");
                break;
            case 11 : System.out.println(sentence + "November");
                break;
            case 12 : System.out.println(sentence + "December ");
                break;
            default : System.out.println("Invalid Number");
        }
    }
}
 



```


### Python :

```python
x = int(input("Please enter the no. of your month: \n"))
 
sentence = "The name of the month according to your number is:"
match x:
    case 1:
        print(f"{sentence} January")
    case 2:
        print(f"{sentence} February")
    case 3:
        print(f"{sentence} March")
    case 4:
        print(f"{sentence} April")
    case 5:
        print(f"{sentence} May")
    case 6:
        print(f"{sentence} June")
    case 7:
        print(f"{sentence} July")
    case 8:
        print(f"{sentence} August")
    case 9:
        print(f"{sentence} September")
    case 10:
        print(f"{sentence} October")
    case 11:
        print(f"{sentence} November")
    case 12:
        print(f"{sentence} December")  

```

# 20.Prime or not (input from the user)


## Exercise
Print if a number is prime or not (Input n from the user). (without creating a method or recursion using if else and for loop or do while loop only)


## Approach:
```javascript
 Note : To find if a number is prime, why is checking till n/2 ?
            
Well, whenever you find a number which is Prime or not , you check it till n/2. That is true, and there is no problem checking it till n. But we don’t check it because there is no possibility of getting a number x which is divisible by n and which lies on the second half of the number (n/2).
 
Let’s check what I am talking about.
 
Consider the number 17. Check whether it is prime or not.
 
17%2≠0 (%=Modulus or Remainder)
 
17%3≠0
 
17%4≠0
 
17%5≠0
 
17%6≠0
 
17%7≠0
 
17%8≠0
 
17%9≠0 (Consider this which lies on the second half in the n/2).
 
You won’t find any more numbers which can produce the result.
 
The minimum number that can be divided by 17 is 2, and if you divide 17/9 which can’t give you the number which is less than 2. (We don’t consider 1 as minimum since 1 is divisible with every other number).
 
So, it is a waste of time to check further for any other number, or it is an inefficient algorithm in terms of computer programming.
 
 
 
Python : 
1st approach = Just same as Java approach mentioned above
 
2nd Approach = In python we can simply use pip(package manager)  to install a python package which is called “sympy” , just go to your terminal(for windows CMD or Powershell or Windows Terminal for Win 11, system terminal for MaxOS and any Linux Based OS) and type “pip install sympy”, it will automatically download and install sympy. After that, type “from sympy import *” on your IDE (see the 1st line of the python solution mentioned below). Then we can use the isprime() method which we imported from sympy !
 
P.S. To uninstall any kinda pip package just type “pip uninstall package_name”
```
<p align="center">
        <img src="https://github.com/Subham-Maity/java-python-problem-solving-series/blob/master/Image(ignore)/20.png?raw=true"/>
        </p>
    
## Solution

### Java :

```java
 
import java.util.Scanner;
class CodeXam {
    public static void main(String[] args) {
        boolean isPrime = false;
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter any number to check prime or not:");
        int n = sc.nextInt();
 
        if (n == 1 || n ==0) {
            System.out.println(n + " is not prime number");
        } else {
            for (int i = 2; i <= n / 2; ++i) {
                // condition for non-prime number
                if (n % i == 0) {
                    isPrime = true;
                    break;
 
                }
            }
            if (!isPrime)
                System.out.println(n + " is a prime number.");
            else
                System.out.println(n + " is not a prime number.");
        }
    }
}
 



```


### Python :

```python
 
num = int(input("Enter Your Number :\n"))
if num > 1:
 
    for i in range(2, int(num / 2) + 1):
        if (num % i) == 0:
            print(num, "is not a prime number")
            break
    else:
        print(num, "is a prime number")
 
else:
    print(num, "is not a prime number")
 
 
#2nd approach
from sympy import *
 
x = int(input("Enter a number to check whether it's a Prime number or not:\n"))
 
if isprime(x):
    print(x, "is a prime number indeed")
else:
    print(x, "is not a prime number ")

```

# 21.Pass or fail

## Exercise
Write a program to find out whether a student is pass or fail; if it requires a total of 40% and at least 33% in each subject to pass. Assume 3 subjects and take marks as input from the user

## Approach:
```javascript
So here we did like this
         
        avg = (subject1 + subject2 + subject3)/3.0
        If Conditions: avg>=40 && subject1>=33 && subject2>=33 && subject3>=33
           print"Congratulations, You have been promoted"
        Else print"Sorry, You have not been promoted! Please try again."


```
## Solution

### Java :

```java
import java.util.Scanner;
class CodeXam
{
    public static void main(String [] args)
    {
        byte m1, m2, m3;
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter your marks in Physics");
        m1 = sc.nextByte();
 
        System.out.println("Enter your marks in Chemistry");
        m2= sc.nextByte();
 
        System.out.println("Enter your marks in Mathematics");
        m3 = sc.nextByte();
        float avg = (m1+m2+m3)/3.0f; //you can do this also Marks Percentage = (What is the total number you got in the exam / The sum of the all subjects highest number ) X 100
       
        System.out.println("Your Overall percentage is: " + avg);
        if(avg>=40 && m1>=33 && m2>=33 && m3>=33){
            System.out.println("Congratulations, You have been promoted");
        }
        else{
            System.out.println("Sorry, You have not been promoted! Please try again.");
        }
    }
}



```


### Python :

```python
physics = int(input("Enter your score in Physics:\n"))
chemistry = int(input("Enter your score in Chemistry:\n"))
mathematics = int(input("Enter your score in Mathematics:"))
 
result = (physics+chemistry+mathematics) / 3
print("\nYour overall percentage is", result)
if result >= 40 and physics >= 33 and chemistry >= 33 and mathematics >= 33:
    print("Congratulations ! You've been promoted ")
else:
    print("Ah , You've failed this year ! See you never :)")
```

# 22.Calculate income tax


## Exercise
```javascript
Calculate income tax paid by you to the government as per the slabs mentioned below:
        
Income Slab	        Tax
2.5L – 5.0L  	        5% 
5.0L – 10.0L 	        20%
Above 10.0L             30%
Note that there is no tax below 2.5L. Take the input amount as input from the user.


```

## Approach:
```javascript
Python : Simple use of if, elif, else methods

```
<p align="center">
        <img src="https://github.com/Subham-Maity/java-python-problem-solving-series/blob/master/Image(ignore)/22.png?raw=true"/>
        </p>


## Solution

### Java :

```java
import java.util.Scanner;
class CodeXam
{
    public static void main(String [] args)
    {
        Scanner sc = new Scanner(System.in);
        System.out.println("Income Slab                 Tax\n" +
                "2.5L –  5.0L                5% \n" +
                "5.0L – 10.0L                20%\n" +
                "Above  10.0L                30%\n" +
                ": Note that there is no tax below 2.5L :\n");
        System.out.println("Enter your annual income ");
        double tax = 0f;
        double income = sc.nextDouble();
        if(income<=250000f){
            tax = tax + 0;
        }
        else if(income>250000f && income <= 500000f){
            tax = tax + 0.05f * (income - 250000f);
        }
        else if(income>500000f && income <= 1000000f){
            tax = tax + 0.05f * (500000f - 250000f);
            tax = tax + 0.2f * (income - 500000f);
        }
        else if(income>1000000f){
            tax = tax + 0.05f * (500000f - 250000f);
            tax = tax + 0.2f * (1000000f - 500000f);
            tax = tax + 0.3f * (income - 1000000f);
        }
 
        System.out.println("The total tax paid by you is: " + tax);
       
 
  }
}



```


### Python :

```python
print("""         Income Slab                Tax
         ============                ====
         2.5L –  5.0L                5%
         5.0L – 10.0L                20%
         Above  10.0L                30%
* Note that there is no tax for income below or equal to 2.5L *""")
 
income = int(input("\nEnter your annual income:\n"))
 
tax1 = (5/100)
tax2 = (20/100)
tax3 = (30/100)
sentence = "Your annual tax is"
 
if income <= 250000:
    print("You have no annual Tax charge !")
elif 250000 < income <= 500000:
    tax = ((income-250000)*tax1)
elif 500000 < income <= 1000000:
    tax = ((500000-250000) * tax1 + (income - 500000)*tax2)
else:
    tax = ((500000-250000) * tax1 + (1000000 - 500000)*tax2 + (income - 1000000)*tax3)
 
print(sentence, tax)

```

# 23.Leap year or not.

## Exercise
Write a program to find whether a year entered by the user is a leap year or not.



## Approach:
```javascript
So here we did like this
Check if the year is divisible by 400 or 4 but not 100, DISPLAY "is a leap year",
Otherwise, DISPLAY ": is not a leap year.""

```
## Solution

### Java :

```java
import java.util.Scanner;
public class CodeXam {
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        int year = sc.nextInt();
        if ((year % 400 == 0) || ((year % 4 == 0) && (year % 100 != 0))) {
            System.out.println(year + " : is a leap year");
        }
        else {System.out.println(year + " : is not a leap year.");
        }
    }
}



```


### Python :

```python
year = int(input("Enter your Year:\n"))
 
leap_year = "It's a leap year !"
common_year = "It's not a leap year"
if year % 4 == 0:
    if year % 100 != 0:
        print(leap_year)
    elif year % 400 == 0:
        print(leap_year)
    else:
        print(common_year)
else:
    print(common_year)

```

# 24.Type of website

## Exercise
* Write a program to find out the type of website from the URL:

* .com – commercial website

* .org – organization website

* .in – Indian website


## Approach:
```javascript
So here we did like this
Java : The Java String class endsWith() method checks if this string ends with a given suffix. It returns true if this string ends with the given suffix; else returns false.
Python : Same like Java, we’re using endswith() method in python as well


```
## Solution

### Java :

```java

import java.util.Scanner;
public class CodeXam {
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter Your Website: ");
        String website = sc.next();
        if(website.endsWith(".org")){
            System.out.println("This is an Organizational website");
        }
        else if(website.endsWith(".com")){
            System.out.println("This is a Commercial website");
        }
        else if(website.endsWith(".in")){
            System.out.println("This is an Indian website");
        }
        }
    }


```


### Python :

```python
user_input = input("Please Enter Your URL:\n")
 
if user_input.endswith(".com"):
    print("It's an Commercial Website")
elif user_input.endswith(".org"):
    print("It's an Organization Website")
elif user_input.endswith(".in"):
    print("It's an Indian Website")
else:
    print("Not Found !")

```

# 25.Email by deleting the part

## Exercise
Input an email from the user. You have to create a username from the email by deleting the part that comes after ‘@’. Display that username to the user.
Example :

email = “codexam@gmail.com” ; username = “codexam”

email = “helloWorld123@gmail.com”; username = “helloWorld123”


## Approach:
```javascript
Python: In python we're simply using slicing, 
we're printing from index 0 to (index of '@') -1

```
<p align="center">
        <img src="https://github.com/Subham-Maity/java-python-problem-solving-series/blob/master/Image(ignore)/25.png?raw=true"/>
        </p>


## Solution

### Java :

```java
import java.util.*;
 
public class CodeXam {
    public static void main(String args[]) {
        System.out.println("Enter Your Gmail");
        Scanner sc = new Scanner (System.in);
        String email = sc.next();
        String userName = "";
 
        /* //You can use this too
 
        for(int i=0; i<email.length(); i++) {
            if(email.charAt(i) == '@') {
                break;
            } else {
                userName += email.charAt(i);
            }
        }
        */
 
        for(int i=0; i<email.length(); i++) {
            if(email.charAt(i) == '@')
                break;
               userName = userName+email.charAt(i);
        }
 
        System.out.println("Your username is: " + userName);
    }
}
 



```


### Python :

```python
user = input("Please enter your email id:\n")
 
x = user.index("@")
 
user_name = user[0:x]
print("Your username is:", user_name)

```

# 1.(Solid Rectangle)

## Exercise
Print the pattern using for loop

<p align="center">
        <img src="https://github.com/Subham-Maity/java-python-problem-solving-series/blob/master/Image(ignore)/1%20p.png?raw=true"/>
        </p>

## Approach:
```javascript
So here we did like this
Row range:0-4 
Column range:0-5
```
<p align="center">
        <img src="https://github.com/Subham-Maity/java-python-problem-solving-series/blob/master/Image(ignore)/1pa.png?raw=true"/>
        </p>

## Solution

### Java :

```java

public class code_xam {
    public static void main(String[] args) {
        for (int i = 1 ; i <=4 ; i++){
            for (int j = 1; j <=5 ; j++){
                System.out.print("*");}
                System.out.println();
            }
        }
    }


```


### Python :

```python
for i in range(1, 5):
    for j in range(1, 6):
        print("*", end=" ")
    print()
```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```

# 

## Exercise


## Approach:
```javascript


```
## Solution

### Java :

```java



```


### Python :

```python

```







