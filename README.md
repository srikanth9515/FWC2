# wc-1
Setup
Installing Apps

    Install F-Droid.
    Open f-droid on your mobile and install the following apps:
        Termux
        Termux:API

Setting up Termux

Give termux access to your user directory in Android.

termux-setup-storage

Upgrade packages (any one command)

pkg upg

apt update && apt upgrade

Install mandatory packages (any one command)

apt install build-essential openssh curl git wget subversion silversearcher-ag imagemagick proot proot-distro python bsdtar mutt nmap neovim

pkg in build-essential openssh curl git wget subversion silversearcher-ag imagemagick proot proot-distro python bsdtar mutt nmap neovim

Installing and Setting up Debian on Termux

Install debian

proot-distro install debian

proot-distro login debian

Inside proot-distro

apt update && apt upgrade

apt install apt-utils build-essential cmake neovim git wget subversion imagemagick nano ranger python3-venv

Installing python3

apt install python3-pip python3-numpy python3-scipy python3-matplotlib python3-mpmath python3-sympy python3-cvxopt

Installing neovim and ranger

apt install neovim ranger libxtst-dev libx11-dev python3-pynvim

    Refer to this document to setup neovim and ranger.
    For usage tips refer to this document.

Installing LaTeX

apt install texlive-full gnumeric

Latex and Python
Latex Template

svn co https://github.com/gadepall/training/trunk/math

texfot pdflatex main.tex

Python

python3 codes/tri_sss.py

Digital Design
Digital Design Book

The book is present here.

To obtain the sources:

git clone https://github.com/gadepall/digital-design

Spoken Tutorials

    Seven Segment Display
    AVR-Assembly
    AVR-GCC

Video Tutorials

The codes used in these videos and relevant references for each video are present at goats-9/fwc-codes. These have been adapted from gadepall/digital-design.

    Arduino/PlatformIO
    AVR-Assembly
    AVR-GCC
    Vaman-ESP32/PlatformIO
    Vaman-FPGA
    Vaman-ARM

fwc-2
Math Computing
Geometry

#The book is present here.

To obtain the sources:

git clone https://github.com/gadepall/geometry

Connecting to Termux via Laptop
SSH

NOTE: Skip this if you are using a bluetooth keyboard

    Follow instructions in Section 1 of the manual.

    On termux on your phone, enter a simple password

    passwd

This command will give you your username

whoami

Find your ip address

ifconfig

Start ssh server on your mobile

sshd

On your laptop, enter the following at a terminal

ssh username@ipaddress -p 8022

    Enter the password and you are connected to termux through your laptop.

Scrcpy

Refer to Genymobile/scrcpy#get-the-app for instructions.
Installing WSL for Windows Users (NOT RECOMMENDED)

Installation instructions are present at this link.

To access USB over WSL, refer to this link.
