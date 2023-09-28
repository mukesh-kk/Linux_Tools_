### Basics Commands on Terminal
- ls: List files and directories in the current directory.
- cd: Change the current directory.
- pwd: Print the current working directory.
- mkdir: Create a new directory.
- touch: Create an empty file.
- rm: Remove files and directories.
- cp: Copy files and directories.
- mv: Move or rename files and directories.

### File Manipulation:

Use cat, less, or more to view the contents of a file.
echo: Display a message or value on the screen.
- '>>' and >: Redirect output to a file (append or overwrite).
- <<: Redirect input from a file.
### Environment Variable
Variables:

- You can create and use variables like my_variable="Hello, World!".
- Access the value of a variable using $my_variable.
- Environment variables, like $HOME and $PATH, store system information.


### Conditionals
Conditionals (if statements):

Use if, elif, and else to create conditional statements.
```
if [ condition ]; then
    # Code to execute if the condition is true
else
    # Code to execute if the condition is false
fi
```

### Case
```
case $variable in
    pattern1)
        # Code to execute if $variable matches pattern1
        ;;
    pattern2)
        # Code to execute if $variable matches pattern2
        ;;
    *)
        # Code to execute if $variable doesn't match any patterns
        ;;
esac

Example
fruit="apple"
case $fruit in
    "apple")
        echo "It's an apple."
        ;;
    "banana")
        echo "It's a banana."
        ;;
    *)
        echo "It's something else."
        ;;
esac

```

### Loops
```
for i in {1..5}; do
    echo "Iteration $i"
done
---
for item in list; do
    # Code to execute for each item in the list
done
---   
count=1
while [ $count -le 5 ]; do
    echo "Count: $count"
    ((count++))
done
---
until [ condition ]; do
    # Code to execute until the condition becomes true
done

```
### Numerical Comparison
Numeric Comparisons:

```
-eq: Equal to (e.g., if [ $a -eq $b ]).
-ne: Not equal to (e.g., if [ $a -ne $b ]).
-lt: Less than (e.g., if [ $a -lt $b ]).
-le: Less than or equal to (e.g., if [ $a -le $b ]).
-gt: Greater than (e.g., if [ $a -gt $b ]).
-ge: Greater than or equal to (e.g., if [ $a -ge $b ]).

```
### Logical Operations
AND (&&) and OR (||)  (! )Operators:
```


Use && for logical AND (e.g., if [ $a -eq 1 ] && [ $b -eq 2 ]).
Use || for logical OR (e.g., if [ $a -eq 1 ] || [ $b -eq 2 ]).


if ! [ -e "$file" ]; then
    echo "File does not exist."
fi

```

### User Input 
Use read 
```

echo "Please enter your name: "
read  name
read -s password
echo "Hello, $name! Welcome."

```

### Arguments to file 
```
Arguments passed to the file  are accessible by special variables $1,$2, etc.

```
 $1 represents the first argument, $2 the second, and so on.
echo "The first argument is: $1"
echo "The second argument is: $2"
echo "The third argument is: $3"

```
