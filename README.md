# Java Journey, 04: If-Else Conditions, Ternary Statements, and Switch Statements

This repository covers the basic control flow structures in Java, which include if-else conditions, ternary statements, and switch statements. These constructs help programmers to make decisions and control the program flow based on the given conditions.

## Study the use of if-else conditions in Java.

In Java, if-else statements are used to execute different code blocks based on certain conditions. The if statement is the most basic conditional statement and is used to execute a block of code if a certain condition is true. The else statement is used to execute a block of code if the condition in the if statement is false.

```bash
int age = 20;

if (age >= 18) {
    System.out.println("You are an adult.");
} else {
    System.out.println("You are not an adult.");
}
```

In this example, if the age variable is greater than or equal to 18, the "You are an adult." message is printed. If it is less than 18, the "You are not an adult." message is printed.

The else-if statement, also known as the else-if ladder, is used to test multiple conditions, with each condition being tested sequentially until one of them evaluates to true. Once a true condition is found, the code block associated with that condition is executed and the rest of the else-if ladder is skipped.

The if-else ladder is a series of if-else statements that are nested together, each one testing a specific condition. The first if statement is executed, and if its condition is true, the corresponding block of code is executed and the rest of the ladder is skipped. If the condition is false, the next else-if statement is tested, and so on, until the final else statement is reached, which is executed if none of the conditions are true.

```bash
int score = 75;

if (score >= 90) {
    System.out.println("You got an A.");
} else if (score >= 80) {
    System.out.println("You got a B.");
} else if (score >= 70) {
    System.out.println("You got a C.");
} else {
    System.out.println("You failed.");
}

```

In this example, the score variable is tested against multiple conditions. If the score is greater than or equal to 90, the "You got an A." message is printed. If it is between 80 and 89, the "You got a B." message is printed, and so on, until the final else statement is reached, which is executed if none of the conditions are true.

A nested if-else statement is a conditional statement that contains one or more if-else statements inside the body of another if-else statement. It allows for more complex decision making in a program. The general syntax for a nested if-else statement in Java is:

```bash
if (condition1) {
  // statements
  if (condition2) {
    // statements
  } else {
    // statements
  }
} else {
  // statements
}

```

The if-else ladder can be used to test multiple conditions and execute different blocks of code depending on the results. It's often used when there are a large number of conditions that need to be tested, or when the conditions are too complex to be handled with a simple if-else or else-if statement.

## Learn about ternary statements and their use.

In Java, the ternary operator, also known as the conditional operator, provides a shorthand way of writing if-else statements. The syntax for the ternary operator is:

```bash
(condition) ? value1 : value2
```

If the condition is true, the operator returns value1, otherwise it returns value2.

The ternary operator is often used in situations where you need to assign a value to a variable based on a condition. For example, consider the following code:

```bash
int x = 10;
int y = (x > 5) ? 1 : 0;
```

In this example, the ternary operator is used to assign the value 1 to y if x is greater than 5, and 0 if it is not.

The ternary operator can also be used in conjunction with method calls, as shown in the following example:

```bash
String result = (x > 5) ? "x is greater than 5" : "x is less than or equal to 5";
System.out.println(result);
```

In this example, the ternary operator is used to assign the appropriate message to the result variable based on the value of x.

Ternary statements are useful when you want to write a simple, concise code that evaluates a single expression and returns a value based on the result. It can be used to make your code more readable and easier to understand, especially when the logic is straightforward and not too complex. However, they can be difficult to read and understand if they are too complex or nested too deeply, so it is important to use them judiciously.

## Get an understanding of switch statements in Java.

In Java, a switch statement is a type of control flow statement that is used to execute code blocks based on the value of a variable or an expression. It provides a concise way to write multiple if-else statements for the same variable.

The syntax of a switch statement in Java is as follows:

```bash
switch (variable/expression) {
    case value1:
        // code block
        break;
    case value2:
        // code block
        break;
    ...
    default:
        // code block
        break;
}
```

Here, the 'variable/expression' is evaluated and the code block corresponding to the matching 'case' statement is executed. If there is no matching 'case' statement, the code block in the 'default' statement is executed. The 'break' statement is used to exit the switch block and continue execution at the statement after the switch block.

Switch statements are useful when there are many possible execution paths for a given value or expression, and when the execution path depends on a limited number of values. They are often used in place of long if-else statements to make the code more readable and easier to understand.

Here's an example of a switch statement in Java:

```bash
int day = 2;
String dayName;

switch (day) {
    case 1:
        dayName = "Monday";
        break;
    case 2:
        dayName = "Tuesday";
        break;
    case 3:
        dayName = "Wednesday";
        break;
    case 4:
        dayName = "Thursday";
        break;
    case 5:
        dayName = "Friday";
        break;
    case 6:
        dayName = "Saturday";
        break;
    case 7:
        dayName = "Sunday";
        break;
    default:
        dayName = "Invalid day";
        break;
}

System.out.println("The day is " + dayName);
```

In this example, the value of day is evaluated and the corresponding dayName is assigned to the variable based on the matching case statement. If day does not match any of the case statements, the default statement is executed and the dayName is set to "Invalid day". The final line of code prints out the value of dayName.

## Difference between If-else statements and switch statements

Both if-else statements and switch statements are used to execute different code blocks based on the condition or value of a variable. However, there are some differences between the two:

- Syntax: The syntax of if-else statements is more flexible and can accommodate a wider range of conditions, while the syntax of switch statements is more rigid and can only be used for certain types of conditions.

- Number of conditions: If-else statements can handle any number of conditions, while switch statements are designed to handle a limited number of conditions.

- Readability: If-else statements can be more readable and easier to understand, especially when there are complex conditions, while switch statements can be more concise and easy to read when there are multiple options.

- Execution time: If-else statements can be slower to execute when there are many conditions, while switch statements are typically faster when there are several conditions to evaluate.

In general, if-else statements are more flexible and can be used in a wider variety of situations, while switch statements are more limited in their use but can be more concise and efficient in some cases. The choice between the two depends on the specific situation and the programmer's preferences.
