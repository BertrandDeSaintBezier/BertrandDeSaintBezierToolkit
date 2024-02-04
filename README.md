# Bertrand-de-Saint-Bezier Toolkit

## GCC for Windows

#### MSYS2 Shell

After installing MSYS2, download gcc and the toolchains for all groups. This will take a minute to download and finish installing.

- Mingw-w64 GCC : `pacman -S mingw-w64-ucrt-x86_64-gcc`
- Mingw-w64 Toolchain : `pacman -S --needed base-devel mingw-w64-x86_64-toolchain`

#### Environment Variable

The following must be added to the System Environement Variables alongside the other **Path** variables : `C:\msys64\mingw64\bin`
You can check that the installation has succeeded by typing `gcc --version` into a git bash terminal.

## Setting up NeoVim

### NeoVim Configuration
 
First off, a decent terminal is required. Don't go with GitBash/Git for Windows as it uses its own installation of Vim (not NeoVim). [Windows Terminal](https://apps.microsoft.com/detail/9N0DX20HK701?hl=en-US&gl=US) is a good alternative.

Run `config_neovim.bat` to create all the necessary config files. By default, this will copy the contents of `config_files/nvim` into `%LOCALAPPDATA%/nvim`.

Start `nvim .` from the Windows Terminal and run `:PackerSync` to retrieve plugins.
