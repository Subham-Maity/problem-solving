# JAVA- Python Problem Series For Beginners
## I cover all type of problems of Java-Python from Basic to Pro Level
# Writer Intro
I am **Subham Maity.**

**Welcome to this book on "Learning HTML In 4 Steps".
I love Programming. One of the aims I had when I started ```CodeXam``` was to make learning programming easy.**

**At ```CodeXam```, we ask ourselves one question every day: "How do we create awesome learning experiences?"**

### Help us improve this guide - Fork, Pull Requests, Shares and Likes are recommended!
## Chapters
*******

### Problem List 
* [**1.Board Percentage Calculator :**](#1board-percentage-calculator-)


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
#4. Asks the user to enter his/her name and greets them with “Hello <name>, have a good day” text.

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



