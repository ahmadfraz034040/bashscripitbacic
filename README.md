Bash Script Basics in Linux 🐧

Overview

Bash scripting is a powerful method for automating tasks in Linux environments. It enables system administrators, DevOps engineers, and developers to organize commands in a file and execute them as a script.

Objectives

By completing this practice, you will learn how to:

- Understand the fundamentals of shell and Bash scripting
- Create and execute Bash scripts
- Use variables and commands
- Accept and process user input
- Automate routine Linux tasks
- Implement conditional statements and loops

What is Bash?

Bash (Bourne Again Shell) is a command-line interpreter commonly used in Linux systems. It enables users to interact with the operating system and automate repetitive tasks.

Creating a Bash Script

Create a file:

nano script.sh

Add the Bash interpreter:

#!/bin/bash

Grant execution permission:

chmod +x script.sh

Run the script:

./script.sh

Basic Bash Commands

Print Output

echo "Hello Linux"

Check the Current User

whoami

Display the Date

date

Display the Current Directory

pwd

Variables in Bash

Example:

#!/bin/bash

name="Ahmad"

echo "My name is $name"

Accepting User Input

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
read| Accept user input
chmod| Modify file permissions
mkdir| Create a directory
cp| Copy files
mv| Move files
rm| Remove files
grep| Search text
tar| Archive and back up files

Practical Learning

During this practice, I learned how Bash scripting enables Linux administrators to automate tasks such as:

- User management
- Backup operations
- System monitoring
- File management
- Server administration

Conclusion

Bash scripting is an essential skill for Linux administrators and DevOps engineers. It improves productivity by minimizing manual effort and automating routine system operations.
