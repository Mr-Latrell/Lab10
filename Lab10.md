## Lab 10

- Name: Keonje Paige
- Email: paige.34@wright.edu

## Part 1 - Compilers

Your Operating System:

Windows PowerShell

Your AWS instance's Operation System:

Ubuntu

- Java
   - How to install on your OS:
sudo apt install default-jdk
   - How to install on OS on AWS: 
sudo apt install default-jdk-y
- C++
   - How to install on your OS:
install apt install g++
   - How to install on OS on AWS:
sudo apt install g++ -y 
- Python
   - How to install on your OS:
sudo apt install python3
   - How to install on OS on AWS: 
sudo apt install python3 -y

Web based IDEs: 

- Java
Replit, JDoodle, GitHub Codespaces
- C++
Pizza.io, Replit, OnlineGDB
- Python
Replit, Jupyter Notebook, Google Colab
## Part 2 - Compiling

1. Method & command to get a copy of the source code files:
 git clone https://github.com/pattonsgirl/CEG2350.git ~/Lab10
2. Command(s) to install the C/C++ compiler on Ubuntu:
sudo apt install build-essential
3. Command(s) to confirm the installation of the C/C++ compiler on Ubuntu:
gcc --version
g++ --version
4. Command(s) to compile the source code into an executable program:
g++ -o TodoList main.cpp utility.cpp
5. Command(s) to execute the program:
./TodoList

## Part 3 - Document

### Program User Guide
TodoList
#### Program Description
This is a to-do list that helps
add, view,and delete certain tasks, 
as well as exit the program. When 
opening the command, it will display
menu like layout.
#### How to Build and Run Program
gtt -o List main.cpp utility.cpp
./TodoList
#### How to Use Program
It display four options for the user
in numerical order:
1. Add Task
2. View Tasks
3. Delete Task
4. Exit
### `git` `branch` Guide

Create a branch:
git branch tasks
Change to branch:
git checkout tasks
Add branch to remote if created locally (GitHub):

Steps to `merge` changes to another branch (`main`):
git checkout main
Steps to resolve a `merge` conflict: 
git merge tasks
## Part 4 - `makey makey`

Using `Makefile` to build executable:
make build will lead to the usage of the following:
build: $(SRC)
        $(CXX) $(CXXFLAGS) -o $(EXEC) $(SRC)
Using `Makefile` to run program:
make run will lead to helping 
executing the following:
run: build
        ./$(EXEC)
Using `Makefile` to remove compilation files, such as the executable: 
make clean will lead to the following:
clean:
        rm -f $(EXEC)
## Extra Credit - Ignore That

Remove this statement and the exclamation point from the line below so TAs can click to check for a working `.gitignore` file.  Test that the link works - if it doesn't, fix the pathing.

![`.gitignore` file in root of repository](../.gitignore)
