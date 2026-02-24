# Bandit Level 0

## Goal
Log into the Bandit game server using SSH. 
> SSH (Secure Shell) is a protocol used to securely connect to a remote computer over a network. It enables logging into remote servers, executing commands remotely, transferring files securely, and encrypts all communication between your local machine and the remote system. In the Bandit wargame, SSH is how we access the remote Linux machine where each level is hosted.
> 
Find the password for the next level (`bandit1`).

## Level Information
**Host:** bandit.labs.overthewire.org  
**Port:** 2220 

**Username:** bandit0  
**Password:** bandit0

## Walkthrough
- To connect to the remote server, use the `ssh` command:
```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```
> Here, `bandit.labs.overthewire.org` is the address of the remote computer we want to access, and `-p 2220` specifies the SSH port to use (SSH normally uses port 22, but Bandit uses 2220). The part `bandit0@` tells the server which username we are logging in as, and when prompted, we enter the password `bandit0` to authenticate. Once the connection is successful, we gain access to the remote terminal and can begin exploring the level.

- When prompted, enter the password for the user `bandit0`:
```bash
bandit0
```

- If the login is successful, you are now in the home directory of `bandit0`.  

- To see the contents of the directory, run:
```bash
ls
```
> The `ls` command lists all the files and directories in your current location.

- You should see a file named `readme`. To view its contents, run:
```bash
cat readme
```
> The `cat` command (short for "concatenate") displays the contents of a file in the terminal.

- Inside the file, you will find the password for the next level (`bandit1`):
```bash
ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
```
