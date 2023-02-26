---
layout: page
title: Setup
---

# Overview

This workshop is designed to be run on pre-imaged Amazon Web Services (AWS) instances.
All of the data and most of the software used in the workshop are hosted on an
Amazon Machine Image (AMI).
Some additional software, detailed below, must be installed on your computer.

Please follow the instructions below to prepare your computer for the workshop:

## Required additional software

This lesson requires a working spreadsheet program.
If you don't have a spreadsheet program already, you can use LibreOffice.
It's a free, open source spreadsheet program.
Directions to install are included for each Windows, Mac OS X, and Linux systems below.
For Windows, you will also need to install either Git Bash, PuTTY, or the Ubuntu Subsystem; you
will use one of these to create a shell session with the remote AMI instance (essentially,
a computer running on Amazon's infrastructure).

> ## Windows
> - IF YOU ALREADY HAVE A SPREADSHEET PROGRAM, YOU CAN SKIP THIS STEP.  But if you need a spreadsheet
program:
>     - Visit [the LibreOffice installation page](https://www.libreoffice.org/download/libreoffice-fresh/).
>   The version for Windows should automatically be selected.
>   Click Download Version X.X.X (whichever is the most recent version).
>   You will go to a page that asks about a donation, but you don't need to make one.
>   Your download should begin automatically.
>     - Once the installer is downloaded, double click on it and LibreOffice should install.
> - Download the [Git for Windows installer](https://git-for-windows.github.io/).
>   Run the installer and follow the steps below:
>   + Click on "Next" four times (two times if you've previously installed Git).
>     You don't need to change anything in the Information, location, components, and start menu screens.
>   + **From the dropdown menu select "Use the Nano editor by default"
>     (NOTE: you will need to scroll up to find it) and click on "Next".**
>   + On the page that says "Adjusting the name of the initial branch in new repositories",
>     ensure that "Let Git decide" is selected.
>     This will ensure the highest level of compatibility for our lessons.
>   + Ensure that "Git from the command line and also from 3rd-party software"
>     is selected and click on "Next".
>     (If you don't do this Git Bash will not work properly,
>     requiring you to remove the Git Bash installation,
>     re-run the installer and to select the
>     "Git from the command line and also from 3rd-party software" option.)
>   + Ensure that "Use the native Windows Secure Channel Library" is selected and click on "Next".
>   + Ensure that "Checkout Windows-style, commit Unix-style line endings" is selected and click on "Next".
>   + **Ensure that "Use Windows' default console window" is selected and click on "Next".**
>   + Ensure that "Default (fast-forward or merge) is selected and click "Next"
>   + Ensure that "Git Credential Manager Core" is selected and click on "Next".
>   + Ensure that "Enable file system caching" is selected and click on "Next".
>   + Click on "Install".
>   + Click on "Finish".
>   + Check the settings for you your "HOME" environment variable.
>     - If your "HOME" environment variable is not set (or you don't know what this is):
>     - Open command prompt (Open Start Menu then type `cmd` and press [Enter])
>     - Type the following line into the command prompt window exactly as shown: `setx HOME "%USERPROFILE%"`
>     - Press [Enter], you should see `SUCCESS: Specified value was saved.`
>     - Quit command prompt by typing `exit` then pressing [Enter]
> - An **alternative option** is to [install PuTTY](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html).
>   For most newer computers, click on putty-64bit-X.XX-installer.msi to download the 64-bit version.
>   If you have an older laptop, you may need to get the 32-bit version putty-X.XX-installer.msi.
>   If you aren't sure whether you need the 64 or 32 bit version,
>   you can [check your laptop version](https://support.microsoft.com/en-us/help/15056/windows-32-64-bit-faq).
>   Once the installer is downloaded, double click on it, and PuTTY should install.
> - **Another alternative option** is to use the Ubuntu Subsystem for Windows.
>   This option is only available for Windows 10 - the Microsoft documentation provides
>   [detailed instructions for installing Windows 10](https://docs.microsoft.com/en-us/windows/wsl/install-win10).
{: .solution}

> ## Mac OS X
> - IF YOU ALREADY HAVE A SPREADSHEET PROGRAM, YOU CAN SKIP THIS STEP.  But if you need a spreadsheet
program:
>   - Visit [the LibreOffice installation page](https://www.libreoffice.org/download/libreoffice-fresh/).
>   The version for Mac should automatically be selected.
>   Click Download Version X.X.X (whichever is the most recent version).
>   You will go to a page that asks about a donation, but you don't need to make one.
>   Your download should begin automatically.
>   - Once the installer is downloaded, double click on it and LibreOffice should install.
{: .solution}

> ## Linux
> - Visit [the LibreOffice installation page](https://www.libreoffice.org/download/libreoffice-fresh/).
>   The version for Linux should automatically be selected.
>   Click Download Version X.X.X (whichever is the most recent version).
>   You will go to a page that asks about a donation, but you don't need to make one.
>   Your download should begin automatically.
> - Once the installer is downloaded, double click on it and LibreOffice should install.
{: .solution}

## Using the lessons with Amazon Web Services (AWS)

This Genomics Data Carpentry workshop will use an AWS AMI instance, but
you do *not* need to worry about setting up an AMI instance yourself.
The Carpentries staff will create an instance for you and this will be provided to you at no cost.
Your Instructor will provide instructions for connecting to the AMI instance at the workshop.

If, outside of this workshop, you would like to work through these lessons independently, 
you can start your own AMI instance by following these 
[instructions on creating an Amazon instance](https://datacarpentry.org/genomics-workshop/AMI-setup/).
Use the AMI `ami-04dd77cd58b3ec654` (Data Carpentry Genomics with R 4.2)
listed on the Community AMIs page.
Please note that you must set your location as `N. Virginia` in order to access this community AMI.
You can change your location in the upper right corner of the main AWS menu bar.
The cost of using this AMI for a few days,
with the t2.medium instance type is very low (about USD $1.50 per user, per day).
Data Carpentry has *no* control over AWS pricing structure and provides this
cost estimate with no guarantees.
Please read AWS documentation on pricing for up-to-date information.

## Using the lessons on your local machine

If, outside of this workshop, you wish to work through the lessons on your local machine
(i.e. without using AWS), please follow the instructions under "Option B" at this link:
[https://datacarpentry.org/genomics-workshop/setup.html](https://datacarpentry.org/genomics-workshop/setup.html)


### IGV

During the Data Wrangling and Processing for Genomics lesson, we will be using a tool called
IGV to view our alignment in a genome browser.  You can save time during the workshop
by installing it in advance:

- [Download the IGV installation files](https://software.broadinstitute.org/software/igv/download)
- [Install and run IGV using the instructions for your operating system](https://software.broadinstitute.org/software/igv/download).
