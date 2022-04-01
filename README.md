# JAVA- Python Problem Series For Beginners
## I cover all type of problems of Java-Python from Basic to Pro Level
# Writer Intro
## **[Subham Maity](https://github.com/Subham-Maity)** who is contributing on **Java** part
## **[Subhasish Negel](https://github.com/Subhasish-Negel)** who is contributing on **Python** part


**Welcome to this book on "Learning JAVA- Python Problem Series For Beginners".
I love Programming. One of the aims I had when I started ```CodeXam``` was to make learning programming easy.**

**At ```CodeXam```, we ask ourselves one question every day: "How do we create awesome learning experiences?"**

### Help us improve this guide - Fork, Pull Requests, Shares and Likes are recommended!

### [Raw Document](https://docs.google.com/document/d/1PzsEHJE54b2QDDNra34MY7-9XOabJOct7ffi0-ywiuk/edit?usp=sharing)
## Chapters
*******

### Problem List 
* [**1.Board Percentage Calculator :**](#1board-percentage-calculator-)
* [**2.Sum of three numbers :**](#2sum-of-three-numbers-)
* [**3.Calculate CGPA :**](#3calculate-cgpa-)
* [**4.Asks the user to enter his/her name and greets them with “Hello , have a good day” text.**](#4asks-the-user-to-enter-hisher-name-and-greets-them-with-hello-name-have-a-good-day-text)
* [**5.Convert Kilometers to miles**](#5convert-kilometers-to-miles)
* [**6.Detects whether a number entered by the user is an integer or not.**](#6-detects-whether-a-number-entered-by-the-user-is-an-integer-or-not)
* [**7.Multiplication table, from any number to any number**](#7-multiplication-table-from-any-number-to-any-number)
* [**8.(Type Casting) Encrypt a grade by adding a number to it. Decrypt it to show the correct grade.**](#8-type-casting-encrypt-a-grade-by-adding-a-number-to-it-decrypt-it-to-show-the-correct-grade)
* [**9.Comparison operators to find out whether a given number is greater than the user entered number or not.**](#9comparison-operators-to-find-out-whether-a-given-number-is-greater-than-the-user-entered-number-or-not)
* [**10. Write the following expression in a Java / Python / in your program**](#10-write-the-following-expression-in-a-java--python--in-your-program)

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
public class CodeXam {
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


#  4.Asks the user to enter his/her name and greets them with “Hello <name>, have a good day” text.


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



