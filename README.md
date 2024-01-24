# README
## GCC for Windows
##### MSYS2 Shell
Download GCC and the toolchains for all groups. This will take a minute to download and finish installing.
- Mingw-w64 GCC : `pacman -S mingw-w64-ucrt-x86_64-gcc`,  
- Mingw-w64 Toolchain : `pacman -S --needed base-devel mingw-w64-x86_64-toolchain`

##### Environment Variable
The following must be added to the System Environement Variables alongside the other **Path** variables : `C:\msys64\mingw64\bin`
You can check that the installation has succeeded by typing `gcc --version` into a git bash terminal.
