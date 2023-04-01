## Day 4 Task: Basic Linux Shell Scripting for DevOps Engineers.

**Tasks**

- ### Explain in your own words and examples, what is Shell Scripting for DevOps.
    - **Shell scripting** is an important skill for DevOps professionals as it allows them to automate tasks and processes in a Unix or Linux environment.
    - Shell scripts are simply text files containing a series of commands that can be executed by the shell interpreter.
    - Some of the key benefits of shell scripting for DevOps include:
        - **Automation:** Shell scripting allows DevOps professionals to automate repetitive tasks such as server setup, software installation, and deployment, which helps to save time and reduce errors.
        -Customization: Shell scripts can be customized to meet the specific needs of an organization, allowing DevOps teams to tailor their workflows to meet their unique requirements.
        - **Consistency:** By using shell scripts, DevOps teams can ensure that tasks are executed consistently and reliably, regardless of who is performing them.
        - **Portability:** Shell scripts can be easily shared and executed across multiple machines and platforms, making it easier for DevOps teams to work collaboratively and across different environments.
    - Some common shell scripting languages used in DevOps include Bash, Python, and Ruby.


 - ### What is `#!/bin/bash?` can we write `#!/bin/sh` as well?
    - `#!/bin/bash` is called a shebang or hashbang line, which specifies the interpreter that should be used to execute the script. In this case, it specifies that the script should be run using the Bash shell.

   - Yes, it is also possible to use `#!/bin/sh` in the shebang line, which specifies that the script should be run using the default shell on the system. On most Unix and Linux systems, the default shell is also Bash, so using `#!/bin/bash` and `#!/bin/sh` will have the same effect. However, there are some systems where the default shell may be different, such as systems that use the Almquist shell (`#!/bin/sh` is compatible with this shell).

    - In general, it's best to use `#!/bin/bash` if the script relies on Bash-specific features or syntax, and `#!/bin/sh` if the script only uses POSIX-compliant features and should be compatible with a wider range of shells.


 - Write a Shell Script which prints `I will complete #90DaysOofDevOps challenge`
 ```
#!/bin/bash
echo "I will complete #90DaysOfDevOps challenge"
```


 - ### Write a Shell Script to take user input, input from arguments and print the variables.
```
#!/bin/bash

# Get input from command-line arguments
arg1=$1
arg2=$2

# Get input from user
echo "Enter a value for variable1:"
read var1
echo "Enter a value for variable2:"
read var2

# Print the variables
echo "arg1 is: $arg1"
echo "arg2 is: $arg2"
echo "var1 is: $var1"
echo "var2 is: $var2"
```


 - ### Write an Example of If else in Shell Scripting by comparing 2 numbers
```
#!/bin/bash

# Define two numbers for comparison
num1=10
num2=20

# Compare the numbers
if [ $num1 -gt $num2 ]
then
  echo "$num1 is greater than $num2"
else
  echo "$num1 is less than or equal to $num2"
fi
```