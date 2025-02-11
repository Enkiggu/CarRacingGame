# Game Project

This project is a terminal-based game written in C++ that utilizes the `ncurses` library for text-based user interfaces. It is designed to work on both **Windows** and **Linux** platforms. Follow the instructions below to compile and run the game on each platform.

---

## Prerequisites

To run this game, you need to have the `ncurses` library installed on your system. The steps vary depending on whether you're using **Linux** or **Windows**.

### Linux

On Linux, you can install `ncurses` easily using your package manager.

1. **Install ncurses library**:
   - For Debian/Ubuntu-based distributions:
     ```bash
     sudo apt-get install libncurses5-dev libncursesw5-dev
     ```
   - For Fedora/RHEL-based distributions:
     ```bash
     sudo dnf install ncurses-devel
     ```

2. **Compile the C++ code**:
   Once `ncurses` is installed, navigate to the directory where `game.cpp` is located and run the following command to compile the code:
  ```bash
  g++ -o game game.cpp -lncurses
  ```
3. **Run the game: After compiling, run the game using**:
  ```bash
  ./game
  ```

### Windows

On Windows, the process is a bit different since ncurses is not natively available. To run this game on Windows, you will need to install a compatible library, such as PDCurses (a Windows-compatible version of ncurses).

Steps for Windows:

1. **Install PDCurses**:

- Download the latest version of PDCurses from here.
- Follow the instructions in the repository to build and install PDCurses for your Windows environment.
- Set up your environment:

- You need a C++ compiler such as MinGW or Visual Studio for Windows. For MinGW, you can use MSYS2 or MinGW-w64.
- **Compile the C++ code: Assuming you have PDCurses installed and the MinGW compiler is available in your path, navigate to the directory where game.cpp is located and run**:
  ```bash
  g++ -o game game.cpp -lpdcurses
  ```
2. **Run the game: After compiling, run the game using**:
  ```bash
  ./game.exe
  ```

## Troubleshooting
- **Missing ncurses/pdcurses libraries**:
  - Ensure that the ncurses or pdcurses libraries are properly installed on your system and that the compiler can find them.
   - On Linux, verify that you have the correct development packages installed.
  - On Windows, ensure that the path to the PDCurses library is correctly set in your environment or specified during compilation.
  - 
- **Compilation errors**:
  - If you encounter any errors related to the ncurses library, double-check your installation process and the command you're using to compile the code.
