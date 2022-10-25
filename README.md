# Compile opencv project via cmake using gcc on windows

## Pre-install
1. Download mingw [here](https://sourceforge.net/projects/mingw-w64/files/), select 8.1.0, x86_64-posix-seh version
2. Extract download file to c:\mingw. Add c:\mingw and c:\mingw\bin to system environment path variable
3. Rebuild opencv using mingw makefiles and mingw-make through cmake gui. Disable opencv precompile header variable, disable tiff related variable (if tiff is not supported). Set module if build opencv with contrib

Command:
```cmd
mkdir build
cd build
cmake .. -G "MinGW Makefiles"
mingw32-make
.\CvEllipseFitExp.exe
```


## References
[1] https://medium.com/csmadeeasy/opencv-c-installation-on-windows-with-mingw-c0fc1499f39  

