We shared all the files on Github. The program 1 is name Exmaples.cpp and the program 2 name Example2.cpp. If users are using the linux environment and want to run the compiled program then type the command: ./<your_program_name>. We used the PALISADE for building our project and ran these files. Users should follow the steps to build and compile the programs. 

Step 1. Build and install PALISADE using “make install”. This will copy the PALISADE library files and header files to the directory chosen for installation.

Step 2.Create the folder for the project on the system. 

Step 3.Copy CMakeLists. Use.txt form the root directory of the git repo to the folder for the project. 

Step 4.Rename CMakeLists.User.txt to CMakeLists.txt. 

Step 5.Update CMakeLists.txt to specify the name of the executable and the source code files. For example, include the following line
add_executable( fhe-demo demo-simple-Examples.cpp )
If using MinGW/Windows(skip this step for other platforms), copy PreLoad.cmke 
Form the root directory of the git repo to the folder for the project. 

Step 6. We create the build directory and cd to it
mkdir build
cd build

Step 7. Run
cmake -DPALISADE_DIR=`<path_to_palisade>` ..

Step 8. Run “make” to build the executable.
