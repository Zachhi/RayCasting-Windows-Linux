# Ray Casting

Simple ray casting simulation that shows how rays of light would behave depending on its source location and the walls around it

**Note: If you have access to Visual Studio, and would prefer that version, it can be found here: https://github.com/Zachhi/RayCasting-VS**

## Demo

(Quality much worse here due to gif-conversion)

![Demo](https://github.com/Zachhi/RayCasting-VS/blob/master/rayCastingDemo.gif)

Watch the video here (above is only a 10 second gif): 
https://www.youtube.com/watch?v=ngBwJ4v9c_M

## Controls

* Click twice to draw a wall from the first click to the second click
* "C" to clear all walls
* Move mouse around to change light source position
* "Space" to change the source type. 
      3 Types:
      Draw all the light rays 
      Draw only the light rays that hit walls
      Draw no light rays
* "Up arrow" to increase amount of light rays
* "Down arrow" to decrease amount of light rays
* "Escape" to exit the program

### Dependencies

* Windows or Linux
* SFML (Simple and Fast Multi-Media Library) 2.5.1 or later. However, I have set everything up already for your convenience. You will not be required to download/link any libraries. The downside is that the download is ~30 MB more.
* GCC 7.3.0 MinGW (32 bit) or later. If you want to use 64 bit version of GCC, download the SFML GCC 64-bit version from https://www.sfml-dev.org/download/sfml/2.5.1/ then simply replace the `include` and `lib` files in `sfmlFiles` with the `include` and `library` files you just downloaded. Then delete and replace the current .dlls with the .dll files in the `bin` folder you just downloaded.
* GNU Make 

**If you want to use Visual Studio, which would not require the use of a makefile (if you dont have GNU Make set up), scroll to the top to find the link**

### Installing And Executing

**Windows or Linux:**
* Download the source code from here, or copy the repository into your enviroment
* Open your terminal
* run the command `make` to build project
* Now run the executable by running the command `run` or `run.exe` to start the program
* If it does not work right away for you, there is two things you have to check:
  * Go to your default compiler path or `C_Cpp.default.compilerpath` and make the path is set to `C:/MinGW/bin/g++.exe` or wherever your MinGW is located
  * Go to your default include path or `C_Cpp.default.includepath` and make sure the path is set to `["${workspaceFolder}**/"]`
  * Run `make` and `run` again and the program should execute

## Authors

Zachary Chi
zachchi@tamu.edu

## License

This project is licensed under the MIT License - see the LICENSE.md file for details
