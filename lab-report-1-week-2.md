**Here is a tutorial for new CSE 15L students.**

1. [Installing VScode](#1)
2. [Remotely Connecting](#2)
3. [Trying Some Commands](#3)
4. [Moving Files with `scp`](#4)
5. [Setting an SSH Key](#5)
6. [Optimizing Remote Running](#6)

---

## <a name="1"></a> Installing VScode
- For this, visit the [VScode website](https://code.visualstudio.com/) and download the application for your respective system
- Once the app is installed, open it up. Travel to your home CSE 15L directory, and open that folder.
- To start doing further commands, open the terminal from the menu bar.

![VS Code](vsScreenshot.png)

## <a name="2"></a> Remotely Connecting
- If you are on Windows or a system without it already, download [OpenSSH](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse)
- Find your CSE 15L specific account details on this [UCSD site](https://sdacs.ucsd.edu/~icc/index.php).
- Enter the following the commands below into the terminal:
    - Type `ssh cs15lwi22XXX@ieng6.ucsd.edu` replacing `XXX` with your account
    - If prompted to, type `yes`
    - Type your password, and you should be able to enter UCSD computer basement servers!

![ssh Command](sshScreenshot.png)

## <a name="3"></a> Trying Some Commands
- Now, try some Unix commands!
- Type `ls` and `ls -a`
- Here are some more:
    - `cd`
    - `ls -lat`
    - `pwd`
    - `mkdir <dirName>`
    - `exit`

![Some Commands](commandsScreenshot.png)

## <a name="4"></a> Moving Files with `scp`
- `scp` stands for secure copy protocol, and allows transfer of files from your system to the server.
- From your system, type `scp <FILE.EXT> cs15lwi22XXX@ieng6.ucsd.edu:~/`, replacing the with a file in your directory and your account. 
- After you enter your password, `ssh` into your account, and type `ls`. You should see your file now on the server!

![Moving Files](scpScreenshot.png)

## <a name="5"></a> Setting an SSH Key
- `ssh` keys will allow us to not use our password everytime we login.
- Follow the commands to generate a key:
    - `ssh keygen`
    - Hit enter twice
- Now, a key pair to login exists. One of these pairs needs to move into the ssh server itself.
    - `ssh` into your account
    - `mkdir .ssh` to make a new .ssh directory
    - `exit`
    - `scp <LOCATION_OF_id_rsa.pub> cs15lwi22XXX@ieng6.ucsd.edu:~/.ssh/authorized_keys` to move the file into your account (replacing the respective words)
    - Now, to test this key-pair, try to `ssh` into your account. You shouldn't need your password!

![Seeing Keys](keyScreenshot.png)

## <a name="6"></a> Optimizing Remote Running
- To make remote running faster and easier to use, here are some helpful tips
    - Use the copy and paste functions to simplify long commands
    - Use `;` to run various commands on the same line
    - Use `"<commands>"` to run various commands together
- Try using VIM or fiddle with your own ways of speeding up the coding process!

![Optimizations](optimizeScreenshot.png)

---
Back to the [homepage](https://nisharu3.github.io/cse15l-lab-reports/)