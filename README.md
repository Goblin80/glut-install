![OpenGL Logo](/images/opengl_logo.jpg?raw=true "OpenGL")

# Glut Installer
A simple batch script that installs *OpenGL Utility Toolkit (GLUT)* over CodeBlocks.

* Run `installglut.bat`

## Manual Installation
If the script fails for any reason, install manually:
1. Copy `glut.h` to CodeBlocks\MinGW\include\GL folder.
1. Copy `glut32.lib` to CodeBlocks\MinGW\lib folder.
1. Copy `glut32.dll` to CodeBlocks\MinGW\bin folder.

## Known Issues
### Multiple undefined references

* Add `#include <windows.h>`
	*(make sure its the **first** declaration)*.
    
### Entry Point Not Found
If you encounter the following message:

![Entry Point Error](/images/entry_point_error.png?raw=true "Entry Point Error")

* Paste a copy of `glut32.dll` beside your executable (.exe) usually found in {ProjectName}\bin\Debug.