
📌 Project Overview

This repository contains basic Bash scripting examples and practical exercises performed in a Linux environment.

Bash scripting is widely used by Linux Administrators, Cloud Engineers, and DevOps Engineers to automate repetitive tasks, manage systems, and improve productivity.

🎯 Learning Objectives

Through this practice, I learned:

- Fundamentals of Shell and Bash scripting
- Creating and executing Bash scripts
- Using variables and user input
- Implementing conditions and loops
- Automating Linux administration tasks
- Writing scripts for system operations

🛠️ Environment

- Operating System: Linux (Ubuntu)
- Shell: Bash
- Editor: Nano / Vim
- Platform: GitHub Repository

📂 Repository Structure

Bash-Scripting-Basics/
│
├── README.md
├── hello.sh
├── variables.sh
├── input.sh
├── conditions.sh
├── loops.sh
├── backup.sh
└── user_management.sh

🚀 Getting Started

Clone Repository

git clone <repository-url>

Navigate to Directory

cd Bash-Scripting-Basics

Give Permission to Execute Script

chmod +x script.sh

Run Bash Script

./script.sh

📚 Bash Script Examples

1. Hello Linux Script

#!/bin/bash

echo "Hello Linux"

2. Variables Example

#!/bin/bash

name="Ahmad"

echo "My name is $name"

3. User Input Example

#!/bin/bash

echo "Enter your name:"
read name

echo "Welcome $name"

4. Conditional Statement

#!/bin/bash

if [ $USER == "root" ]
then
    echo "Root User"
else
    echo "Normal User"
fi

5. Loop Example

#!/bin/bash

for i in 1 2 3 4 5
do
    echo "Number: $i"
done

⚙️ Automation Scripts

Backup Automation

#!/bin/bash

tar -czf backup.tar.gz /home/user/Documents

echo "Backup completed"

User Management Automation

#!/bin/bash

for user in user1 user2 user3
do
    sudo adduser $user
done

🔑 Important Linux Commands Used

Command| Description
echo| Display output
read| Take user input
chmod| Change permissions
mkdir| Create directory
cp| Copy files
mv| Move files
grep| Search data
tar| Backup files
systemctl| Manage services

💡 Skills Gained

✅ Linux Command Line
✅ Bash Automation
✅ File Management
✅ User Management
✅ Backup Automation
✅ DevOps Fundamentals

👨‍💻 Author

Ahmad Fraz

Learning Linux, Cloud Computing, and DevOps Automation.

⭐ Conclusion

Bash scripting is a fundamental skill for Linux and DevOps professionals. This repository demonstrates practical scripting knowledge used for automating daily system administration tasks.
