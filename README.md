# :speech_balloon: UserInput
How gain input from the user through the console. 

Programs can be made more interactive by taking user input from the console.  

`Scanner` is an object that can read input from many sources (files, console, databases, web sites)
It uses `System.in` to communicate (versus `System.out`)

## :fax: Using Scanner 

```
import java.util.*; //this is an import statement to bring make the Scanner accessible within your code

//Constructing a Scanner (we will talk about constructors, when we discuss Objects)

Scanner console = new Scanner(System.in); //we can choose to name it whatever we want versus console.  

```

## `Scanner` methods

|Method|Description|
|------|-----------|
|`nextInt()`|reads an int from the user and returns it|
|`nextDouble()`|reads a double from the user|
|`next()`|reads a one-word String from the user|
|`nextLine()`|reads a one-line String from the user|

The Scanner waits until the user presses Enter.  
The value is then returned to the user.  

### Example 1: 

```
Scanner console = new Scanner(System.in);

//prompt the user
System.out.print("What is your name? "; 
String name = console.nextLine(); 
System.out.println("Your name is: " + name); 

```

### Example 2: 

Division of two integers.  

Note:  The Scanner uses the idea of **tokens** which are inputs separated by whitespace (spaces, tabs, new lines).  
Thus two integers can be entered on the same line and the Scanenr can recognize them as two different tokens. 

```
Scanner console = new Scanner(System.in); 

System.out.print("Please enter a dividend and divisor separated by a space: ); 
int dividend = console.nextInt();
int divisor = console.nextInt(); 

double output = (double) dividend / divisor

System.out.println(dividend + " / " + divisor + " = " + output); 

```

### Scanner Exercises

Rewrite your exercises from the nested for loop exercies we did last class.
1.  Adjusting the pattern of dots and numbers to accomodate any input.  
2.  Adjusting the rectangle accept a user input width and height.  
3.  Adjust the last exercise to accept a user input for size. 
