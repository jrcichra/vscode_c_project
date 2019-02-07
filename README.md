# How to setup C compilation and debugging in VSCode (Windows)

I love VSCode, but C doesn't work out of the box. I did some googling online but didn't come up with  a perfect solution in one place. This guide is by no means perfect, but it should help you get up and running, coding and debugging c programs

## Installation

If you haven't already, install [Visual Studio Code](https://code.visualstudio.com/) for your platform.

Download [MinGW](https://osdn.net/projects/mingw/releases/) with the blue ```mingw-get-setup.exe``` button.

Install MinGW in the default location of C:\MinGW. When MinGW asks you what packages you want to install, do the base C compiler and C++ compiler. In theory, this will work for both, however, as of the current moment, I've only written C code in VSCode.
![](https://i.imgur.com/MNlkRgF.png)

Once this is done, close the MinGW installer.

Open up VSCode and navigate to a new project folder.

Inside this folder, make a .vscode directory.

Inside that .vscode directly, download and place the .json files into the .vscode directory.

![](https://i.imgur.com/O6NHUc9.png)

Inside tasks.json, the "command" is what will be run as part of compilation. Change the gcc line to match your needs. In this case, I have main.c sent to gcc.

![](https://i.imgur.com/It6z8x5.png)

Add gcc to your system environment variable path. You can specify the exact path inside the tasks.json,  but if you ever want to do gcc in cmd, this makes it soooo much nicer.

![](https://i.imgur.com/XjTeH50.png)

![](https://i.imgur.com/oCWfX1K.png)

![](https://i.imgur.com/cjBMh8R.png)

![](https://i.imgur.com/MaILoCc.png)


This "should" be everything you need to get it working. I'll be making the process simpler as we go but this is revision 1. Open up an issue if I missed anything.


Justin

