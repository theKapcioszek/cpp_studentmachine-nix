# STUDENT MACHINE

Project forked from: https://github.com/marcin-filipiak/cpp_studentmachine  
I wanted to make this fork to see how well pairing it up with NixOS would work.  

<br>

## This fork's NixOS VM Features
- graphical environment
- C and C++ compiler
- Python interpreter
- Vscodium (Open Source binaries for vs code) 
- build tools (make, cmake, ninja, meson)
- firefox

<br>

## Todo  

- [ ] add support for LAMP stack like on the original
- [ ] take a look at template and excercise scripts to see if they need updating
- [X] update the manual
- [X] actually upload the vm image and replace the link

<br><br><br>


The "STUDENT MACHINE" program is a tool written in C++ that provides a simple interface for users to manage a programming project on GitHub. Student need to work own github account and repository "student_projects". 

Here's an overview of the program's functionality from the user's perspective:

To run the program, follow these steps:
* Open a terminal.
* Navigate to the directory where the studentmachine executable is located.
* Run the program by typing the following command and providing a parameter:

`studentmachine [command]`

Replace [command] with one of the command.

For example, to install the required tools, you would run:

`studentmachine install`

### Installation and System Setup

Command: `install`

Functionality: Installs necessary software packages and updates the application to the latest version.

### Version Checking and Updating

Command: `update`

Functionality: Checks and updates the application to the latest version from a specified GitHub repository.

### System Initialization and Configuration

Command: `systemup`

Functionality:
- Clears existing student projects and system history.
- Optionally registers GitHub credentials (login and email).
- Downloads and registers SSH keys from a specified keyring.
- Configures Git with the provided GitHub login and email.
- Clones the GitHub repository for student projects.

### Saving Work to Repository

Command: `savework`

Functionality:
- Loads GitHub login and email from configuration files.
- Commits changes to the local Git repository in student_projects.
- Pushes changes to the GitHub repository.

### Template Download and Configuration

Command: `templates`

Functionality: Downloads project templates, runs a script to configure the workspace according to the template, and creates symbolic links.

### Exercise Download and Configuration

Command: `exercise [exercise_name]`

Functionality: Downloads a specific exercise, extracts it, runs a script to configure the exercise, and cleans up after the configuration.

### System Shutdown

Command: `systemdown`

Functionality:
- Loads GitHub login and email from configuration files.
- Commits changes to the local Git repository in student_projects.
- Optionally pushes changes to the GitHub repository.
- Cleans up SSH keys.
- Shuts down the machine.ation files.
- Commits changes to the local Git repository in student_projects.
- Pushes changes to the GitHub repository.

# LINKS

Vitrual Machines:  
[Virtual Machine for VirtualBox 7.0, NixOS with integrated StudentMachine](https://drive.google.com/file/d/1MBZKLquyEwGBDc3X8rH0Rz7RXSJf2DuV/view?usp=sharing)  
[Same machine but with everything already installed](https://drive.google.com/file/d/1C6xTgLLwlpovgp8L-5Gu9N1_UdRu3I16/view?usp=sharing)

Official keyring server for StudentMachine where you can find your public key (need to import in Github)
http://api.noweenergie.org/application/StudentMachine/keyring/
