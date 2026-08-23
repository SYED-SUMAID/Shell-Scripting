# Variables, If-Else Statements & Loops

A simple Linux Shell Scripting lab demonstrating variables, conditional statements, and loops using Bash.

## Objective

The objective of this lab is to understand:

- Shell variables
- User input
- `if`, `elif`, and `else` statements
- `for` loop
- `while` loop
- Basic comparison and arithmetic operators

## Bash Script

```bash
#!/bin/bash

# Variables
name="Sumaid"
age=21
course="Shell Scripting"

echo "===== VARIABLES ====="
echo "Name: $name"
echo "Age: $age"
echo "Course: $course"


# If / Elif / Else
echo
echo "===== IF / ELIF / ELSE ====="

read -p "Enter your marks: " marks

if [ $marks -ge 80 ]; then
    echo "Grade: A"
elif [ $marks -ge 60 ]; then
    echo "Grade: B"
elif [ $marks -ge 40 ]; then
    echo "Grade: C"
else
    echo "Grade: Fail"
fi
     

# For Loop
echo
echo "===== FOR LOOP ====="

for i in {1..5}
do
    echo "Number: $i"
done

# While Loop
echo
echo "===== WHILE LOOP ====="

count=1

while [ $count -le 5 ]
do
    echo "Count: $count"
    ((count++))
done

echo
echo "===== PROGRAM COMPLETED ====="

```
## Conclusion

This lab provided a basic understanding of Linux Shell Scripting by implementing variables, user input, conditional statements, and loops. The use of if, elif, else, for, and while helped demonstrate decision-making and repetition in Bash.