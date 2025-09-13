    # Change Management

    This section outlines the process for managing changes to this project/repository.

    ## Change Log

    | Version | Date       | Description          |
    | ------- | ---------- | -------------------- |
    | 1.0.1   | 2025-09-12 | Minor bug fixes      |
    | 1.0.0   | 2025-09-01 | Initial release      |

    ## How to Propose Changes

    1. Fork the repository.
    2. Create a new branch for your changes.
    3. Make your modifications.
    4. Submit a pull request with a clear description of the changes.

    ---

# How to Install Python with Homebrew
Homebrew is a free and open-source software package management system that simplifies the installation of software on macOS and Linux. This guide will walk you through the steps to install Homebrew, and then use it to install Python 3.

## **Step 1: Install Homebrew**
The first step is to install Homebrew by running the installation script in your terminal.

Open the Terminal app on your Mac. You can find it by going to Applications > Utilities > Terminal.

Copy and paste the following command into your terminal window and press Enter.

This command downloads and runs the Homebrew installation script. The script may ask for your administrator password to proceed with the installation.

/bin/bash -c "$(curl -fsSL [https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh](https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh))"

Follow the on-screen instructions. The script will explain what it's about to do and ask you to confirm before proceeding.

Add Homebrew to your PATH. After the installation is complete, the script will provide two commands to add Homebrew to your shell's PATH. This ensures that you can run brew commands from anywhere in the terminal.

The commands will look something like this:

echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/your-username/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"

Verify the installation. Run the following command to make sure Homebrew is installed correctly.

brew --version

The command should return the version number of your Homebrew installation.

## **Step 2: Install Python 3
With Homebrew installed, you can now use it to effortlessly install Python 3 and other packages.

Install Python 3. Run the following command in your terminal. Homebrew will handle the entire process of downloading, compiling, and installing the latest version of Python 3.

brew install python3

Verify the Python 3 installation. To confirm that Python 3 has been installed, run the following command. The terminal should display the Python version number.

python3 --version

Start using Python 3. You can now use the python3 command to run your Python scripts.

For example, create a simple Python file named hello.py with the following code:

print("Hello, Homebrew!")

Run the script using the following command:

python3 hello.py

The terminal will print the message "Hello, Homebrew!", confirming that Python 3 is working correctly.

Congratulations! You have successfully installed Homebrew and used it to install Python 3. You can now use Homebrew to manage other software packages as you build your development environment.
