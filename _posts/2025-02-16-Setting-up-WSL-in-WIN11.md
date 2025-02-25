---
title: Installing WSL in Win 11 and Setting up ZSH
date: 2025-02-17 00:03:00 -800
categories : [tutorial,tech]
tags: [Windows11,guide]
---
 

# Introduction

Why would you want to set up WSL **(Windows Subsystem for Linux)** well it will allow you to run many Linux Distros without having to go through setting up a Hypervisor, Dual booting, or other virtualization software. While I feel that each one of these tools has a purpose, sometimes you just need to jump into Linux to test something and jump back out. You also have access to your Linux files in your Windows 11 file explorer so that always a plus. So lets get started.

  

## Step 1: Installing WSL

> there are many ways to install WSL this is the one I choose based on documentation from Microsoft.

{: .prompt-tip }

- open PowerShell as admin

- run ```wsl --install```

> this command will install Ubuntu by default for my purposes this is fine.

{: .prompt-tip }

- *If you wish to have a differing distro* to see all available distros enter ```wsl --list --online```
- pick your preferred distro
- Install using ```wsl --install -d <distro>"```. enter the preferred distro in the "distro" field to control what distro is installed.

  

There are many other switches/variables you can use with this command read more about them [here.](https://learn.microsoft.com/en-us/windows/wsl/install)
- Once you've entered the command it will run and download and Install WSL.
- A terminal window will open asking you to set up an account and password.
## Step 2: Set up Ubuntu as your default terminal application
- Click on windows icon and type in **Terminal**, click on app if not already opened
- Click on drop down arrow located on the furthest right tab, then settings 
- In left pane **Startup** should be selected if not select it
- For "Default Profile" option select in my case was Ubuntu, your case may differ. 

## Step 3: Update Ubuntu and Set up Zsh and Oh My Zsh
>  ZSH is not a requirement but I prefer it along  with Oh My Zsh

### Updating Ubuntu
-  lets update the Linux pre installed packages
- enter in 
```sudo apt-get update ```
- the ```sudo apt-get upgrade```
- agree when asked
### Installing ZSH (optional)
- enter the following in terminal 
	- ```apt install zsh```
### Install oh my zsh
- refer to the [documentation]([Oh My Zsh - a delightful & open source framework for Zsh](https://ohmyz.sh/#install)) for the latest install script usually use curl

You are all done setting up your Windows Machine with WSL, using Ubuntu and ZSH. 

An extra step is to install a code editor my choice is usually VS Code. 

Till Next time. 
