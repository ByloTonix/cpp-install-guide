# Installing Qt tools

To develop GUI applications in Qt you need to install the Qt Framework.

The framework is different from Qt Creator. Qt Creator is an IDE with built-in support for the framework and useful tools for working with it. The Qt Framework is a set of libraries and modules that allow you to build a graphical application using any IDE or compiler.

We continue using VS Code, so this guide focuses on installing just the framework and working in VS Code. You may install Qt Creator as well if you want to.

## Qt Framework

### Mac

1. Install Brew if you haven't already - https://brew.sh/
2. Use Brew Formula `brew install qt` - https://formulae.brew.sh/formula/qt

### Windows

1. Install MSYS2 if you haven't already - https://www.msys2.org/
2. Install the Qt6 Base package - `pacman -S mingw-w64-x86_64-qt6-base` - https://packages.msys2.org/package/mingw-w64-x86_64-qt6-base

## Qt Creator

Both Homebrew and MSYS2 have packages for Qt Creator:

https://formulae.brew.sh/cask/qt-creator

https://packages.msys2.org/package/mingw-w64-x86_64-qt-creator

However, Qt Creator requires activation (even for a free license), and you need a VPN for that. You may install Qt Creator but this guide will focus on how to install everything without it.

## Qt Designer (if you haven't installed Qt Creator)

Qt Creator, the IDE, comes with additional tools. One of the tools is Qt Designer which allows you to design applications in the interface instead of by writing code (you drag and drop widgets, set their properties, etc).

You can get a standalone version of Qt Designer here - https://build-system.fman.io/qt-designer-download (both Mac and Windows).


## VS Code

CMake can build applications that use the Qt Framework if you add the right `CMakeLists.txt` file. An example file is included in this project and will be included in future projects uploaded to GitHub.

However, you may want to use additional Qt tools like IntelliSense (inline documentation) and debugging. The VS Code extension `Qt Tools` may help with this - https://marketplace.visualstudio.com/items?itemName=tonka3000.qtvsctools (the extension is unofficial).

