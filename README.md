# Template

## Informations

I've made this project to learn about various techniques of C++/CI/CD/Tests and "modern" Cmake and Github integration.

## Install

To run the project you will need to have :
* A C++17 compiler
* Conan 
* CMake


Now you can run cmake and compile the project :
````bash
$ mkdir build
$ cd build
$ cmake -H.. -B. -G"GENERATOR"  -DCMAKE_INSTALL_PREFIX=../install -DCMAKE_BUILD_TYPE=Debug
$ cmake --build . --target Particles --config Debug
````

If you are on windows, you can also use the .bat scripts in the `tools` folder.

## Optional

Install NSIS https://nsis.sourceforge.io/Download for executable packaging.

## Tests

Run CTest from the build directory, and and pass the desired configuration :

````bash
cd build 
ctest -C Release 
````


## Thanks
Thanks to filipdutescu for the modern cmake template : https://github.com/filipdutescu/modern-cpp-template

I've done some modifications from his work based on my personal experiences. 

And I'm still learning about single_header projects, how to uses matrix in github worklows, test driven programming, code coverage, that kind of stuff.
