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

![Bash terminal displaying the variables section with Name: Sumaid, Age: 21, and Course: Shell Scripting. The screenshot shows a plain command-line environment used for this instructional lab.](<Screenshot (602)(1).png>)
![Bash terminal displaying the IF / ELIF / ELSE section, where the user enters marks and the script displays a grade. The screenshot shows a plain command-line environment demonstrating conditional logic in an instructional setting.](<Screenshot (607).png>)
![Bash terminal displaying the FOR LOOP results: Number: 1, Number: 2, Number: 3, Number: 4, and Number: 5. The screenshot shows repeated output in a plain command-line environment for this instructional lab.](<Screenshot (608).png>)
![Bash terminal displaying the WHILE LOOP results: Count: 1, Count: 2, Count: 3, Count: 4, and Count: 5, followed by PROGRAM COMPLETED. The screenshot shows a plain command-line environment demonstrating repetition in an instructional setting.](<Screenshot (609).png>)

```
##Conclusion

This lab provided a basic understanding of Linux Shell Scripting by implementing variables, user input, conditional statements, and loops. The use of if, elif, else, for, and while helped demonstrate decision-making and repetition in Bash.