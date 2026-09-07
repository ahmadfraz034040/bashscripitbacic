Bash Script Basics in Linux 🐧

Overview

Bash scripting is a powerful way to automate tasks in Linux environments. It allows system administrators, DevOps engineers, and developers to write commands in a file and execute them as a script.

Objectives

By completing this practice, you will learn:

- Basics of Shell and Bash scripting
- Creating and executing Bash scripts
- Using variables and commands
- Taking user input
- Automating routine Linux tasks
- Working with conditions and loops

What is Bash?

Bash (Bourne Again Shell) is a command-line interpreter used in Linux systems. It helps users interact with the operating system and automate repetitive tasks.

Creating a Bash Script

Create a file:

nano script.sh

Add the Bash interpreter:

#!/bin/bash

Give execution permission:

chmod +x script.sh

Run the script:

./script.sh

Basic Bash Commands

Print Output

echo "Hello Linux"

Check Current User

whoami

Display Date

date

Show Current Directory

pwd

Variables in Bash

Example:

#!/bin/bash

name="Ahmad"

echo "My name is $name"

Taking User Input

#!/bin/bash

echo "Enter your name:"
read name

echo "Welcome $name"

Conditional Statements

Example:

#!/bin/bash

if [ $USER == "root" ]
then
    echo "You are root user"
else
    echo "Normal user"
fi

Loops in Bash

For Loop

#!/bin/bash

for i in 1 2 3 4 5
do
    echo "Number: $i"
done

While Loop

#!/bin/bash

count=1

while [ $count -le 5 ]
do
    echo $count
    count=$((count+1))
done

Automation Examples

Backup Script

#!/bin/bash

tar -czf backup.tar.gz /home/user/Documents

echo "Backup completed successfully"

Create Multiple Users

#!/bin/bash

for user in user1 user2 user3
do
    sudo adduser $user
done

Important Bash Commands

Command| Purpose
echo| Display output
read| Take user input
chmod| Change permissions
mkdir| Create directory
cp| Copy files
mv| Move files
rm| Remove files
grep| Search text
tar| Backup files

Practical Learning

During this practice, I learned how Bash scripting helps Linux administrators automate tasks such as:

- User management
- Backup operations
- System monitoring
- File management
- Server administration

Conclusion

Bash scripting is an essential skill for Linux administrators and DevOps engineers. It improves productivity by reducing manual work and automating daily system operations.
