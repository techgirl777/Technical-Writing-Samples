# How to Install Python with Homebrew on MacOS

Homebrew is a free and open-source software package management system that simplifies the installation of software on macOS. This guide will walk users through the steps to install Homebrew, before using it to install Python 3.

## Step 1: Install Homebrew

1. Open the Terminal app on a Mac using the folloowing path: Applications > Utilities > Terminal.
2. Copy and paste the following command into Terminal and press Enter.

```
/bin/bash -c "$(curl -fsSL [https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh](https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh))"
```
> [!NOTE]
> This command downloads and runs the Homebrew installation script from its GitHub repository,
found at [GitHub Homebrew Install](https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh).
> The script may ask for an administrator password to proceed with the installation.

3. Follow the on-screen instructions.

> [!NOTE]
> The script will provide explanations and ask for confirmations before proceeding.

4. Add Homebrew to a local PATH using this command (The PATH will be specific to each user's computer).

```
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/your-username/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```
> [!NOTE]
> After the installation is complete, the script will provide two commands to add Homebrew to the user's shell PATH.
> This ensures that brew commands can be used from anywhere within the Terminal app.

5. Verify the installation by running the following command to display Homebrew's version number.

```
brew --version
```

## Step 2: Install Python 3

With Homebrew installed, it can now be used to effortlessly install Python 3 and other packages.

1. Run the following command to install Python.
   
```
brew install python3
```

> [!NOTE]
> Homebrew will handle the entire process of downloading, compiling, and installing the latest version of Python 3.

2. Confirm that Python has been installed by copying and pasting this code to display Python's version number.

```
python3 --version
```

## Step 3: Start Using Python 3

1. The python3 command can now be used to run Python scripts. Let's try creating a simple Python file named hello.py with the following code.

```
print("Hello, Homebrew!")
```
2. Run the script.

```
python3 hello.py
```

> [!NOTE] 
> Terminal will print the message **"Hello, Homebrew!"**, confirming that Python 3 is working correctly.

Congratulations! Homebrew has been successfully installed and used to install Python 3. Homebrew can now manage software packages for further development environments.
