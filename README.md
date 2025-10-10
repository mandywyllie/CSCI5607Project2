
![Untitled video - Made with Clipchamp](https://github.com/user-attachments/assets/228dad0e-4474-41c6-9381-c951741587b1)
## Difficulties

The hardest part of this project for me was setting up Visual Studio and SDL3. I had never made a blank project before so I had no idea what header files were and how to link external libraries in Visual Studio. I spent a lot of time figuring this out with the help of this video. Once I had the starter code working in Visual Studio, the rest of the project went fairly smoothly. I think this was because most of the functions required for the project could be done using PGA, something I was very familiar with from homework 1. In fact, I was able to use multiple of the functions from my header file from homework 1. I had some trouble with figuring out how to compute the angle between the initial mouse click and the current mouse position. I knew how to find the magnitude of the angle between two lines with PGA, but I had to look up how to find the sign of the angle because with just the magnitude implemented, the square only rotated in one direction. The last difficulty I had was with learning what I had to include in the command line to compile the file as I had never used "-I", "-L", or "-l" before.

## Compiling the Project Locally
Here is a zip file with all files needed to compile my project on windows:
[project1Graphics.zip](https://github.com/user-attachments/files/22585764/project1Graphics.zip)
Extract these zip files to a new folder, and open that folder in windows Terminal or command prompt.
To compile, you must have SDL3 downloaded to the computer, which you can get from [here](https://github.com/libsdl-org/SDL/releases/latest.). Download "
SDL3-devel-3.2.22-VC.zip ", and extract the files to a folder of your choosing (C:\*yourSDLfilepath\*). I extracted the files to a new folder with the location "C\SDL".
On my computer, I can compile the project by running the following line in the command prompt:
```
g++ .\squareStarter.cpp .\glad\glad.c -I C:\SDL\SDL3-3.2.22\include -L C:\SDL\SDL3-3.2.22\lib\x64 -lSDL3 -o project1.exe
```
You want to change "C:\SDL\SDL3-3.2.22\include" and "C:\SDL\SDL3-3.2.22\lib\x64" to have the correct file path on your computer, so this will look like:
```
g++ .\squareStarter.cpp .\glad\glad.c -I C:\*yourSDLfilepath*\SDL3-3.2.22\include -L C:\*yourSDLfilepath*\SDL3-3.2.22\lib\x64 -lSDL3 -o project1.exe
```
This should compile a new executable "project1.exe".

## Running the project/Extra Features
While in the project directory, type "project1.exe" into the command line. Pressing "g" will change the texture of the square between the three textures given in the project starter code.
