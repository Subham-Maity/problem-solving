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
