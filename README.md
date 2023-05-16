# dk-shell-script-basics

## Variables
###Setting Variables
variable_name=variable_value_here
eg:
```
cal_sum=done
```

##Command Line Argument

This help to pass variables from the command line to the script.

Let assume our script is called 'scrpt.sh' and we a variable called 'cal_sum', to pass in the arguments, we need to refernce it by $1

ie:
 ```
 cal_sum=$1
 
``

now run the script with the argument.

```
./script.sh sum


#Read Inputs
It used to take input from the user to insert into a script

eg:
```
read -p "Enter input here" cal_sum

In the real world both READ and COMMAND LINE ARGUMENTS works thesame, but if you running a simple script, then it ok to use the read to ask the user to enter value.

but if its a complex scripts, then the command line args can be used. also if statement can be used to check if user have entered args in the commands line if not usse read to ask for value.


##Arithmetic Operators
```
expr 4 + 5
expr 4 - 5
expr 4 / 5
expr 4 \* 5
expr 4 + 5

```
OR use Echo

echo ((2+4))
echo ((2*4))
echo ((2-4))
echo ((2/4))


##SHELLCHECH

yum install shellchech

to run

shellcheck shell.sh
