## Hi there 👋, I'm Jermell, an [IT Professional!](https://www.linkedin.com/in/jermell-riddick-83b01721b/)

## Information Technology Projects

# Ubuntu Server and Fedora Linux Package Management 

## Project Overview

This project covers a range of tasks from compiling and installing programs from source on Fedora Linux to managing `.deb` packages on an Ubuntu Server. You will use tools like `dnf`, `git`, and `make` for Fedora and `dpkg`, `apt`, and `aptitude` for Ubuntu. This combination of source-built and pre-packaged software management provides a comprehensive look at Linux system administration.

## Key Topics

1. **Cloning and Compiling Programs from Source on Fedora Linux** 
2. **Managing Packages on Ubuntu Server** 
3. **Using Aptitude for Advanced Package Management** 

## Step-by-Step Guide

### Fedora Program Compilation from Source 

In this section, you will learn how to clone, compile, and install software from source code on Fedora Linux.

1. **Install Development Tools:**
    ```bash
    dnf groupinstall "Development Tools"
    ```
    Installs a collection of development and compiler tools from a repository.

2. **Clone a GitHub Repository:**
    ```bash
    git clone https://github.com/bartobri/no-more-secrets.git
    ```
    Clones the `no-more-secrets` program repository.

3. **Navigate to the Project Directory:**
    ```bash
    cd no-more-secrets
    ```

4. **Compile the Program:**
    ```bash
    make nms
    make sneakers
    ```
    These commands use `make` to compile the `nms` and `sneakers` programs using the GNU C compiler.

5. **Install the Compiled Program:**
    ```bash
    make install
    ```
    Installs the programs and any associated files in the appropriate directories.

6. **Clean Up the Cloned Repository:**
    ```bash
    rm -Rf no-more-secrets
    ```
    Removes the cloned repository after the programs are installed.

7. **Verify Installation:**
    ```bash
    which nms sneakers
    ```
    Checks the installation location of the `nms` and `sneakers` executables.

---

### Fedora Linux RPM Package Management 

This part covers basic RPM package management tasks on Fedora Linux, such as:

- Checking installed RPM packages
- Verifying the installation of specific packages (e.g., `ncompress`)
- Listing package information and associated files
- Handling shared library dependencies for executables
- Installing and removing RPM packages
- Searching for and installing packages from the repository using DNF



#### Example Commands Used:
```bash
rpm -qa | less
rpm -q ncompress
rpm -qi ncompress
rpm -e ncompress
dnf install ncompress


