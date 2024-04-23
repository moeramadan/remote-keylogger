# Remote Keylogger

## Project Objective:
The main objective of this project was to design and implement a remote keylogger in Python, with the added functionality of disguising it as a harmless image file. Additionally, the program was developed to facilitate remote transmission of captured keystrokes and included a safety key feature to terminate the keylogging process.

## Features:
- **Stealthy Operation**: The keylogger was designed to operate covertly by disguising itself as an image file, making it difficult to detect.
- **Remote Transmission**: Captured keystrokes were transmitted remotely to a designated email address, allowing for discreet monitoring.
- **Safety Key**: Implemented a safety key feature that provided a secure method to terminate the keylogging process remotely.
- **Host Information Collection**: The program collected essential host information, including hostname, IP, username, saved WiFi profiles, MAC address, and more.

## Code Overview:

## Imports
The project starts with importing essential Python libraries that enable the implementation of various functionalities:

- **tkinter**: Used for creating a graphical user interface (GUI) popup on the screen.
- **pynput.keyboard**: Employed to capture keystrokes efficiently.
- **logging**: Utilized for creating log files to store captured keystrokes.
- **os**: Facilitates interaction with the host operating system (Windows), enabling file operations and system calls.
- **getpass/uuid/socket**: Enables fetching host information such as hostname, IP address, and MAC address.
- **threading**: Used for executing processes in unique threads, ensuring seamless multitasking.
- **subprocess**: Enables running system commands from within the Python program.
  
![image](https://github.com/moeramadan/remote-keylogger/assets/155490852/cd10f782-cfc5-4a8d-a109-8e92194f3dbd)

### Setup:
Began the process by importing Configured SMTP email service and established a temporary file to store all logged keystrokes, disguised as "license_win64_details.txt".

![image](https://github.com/moeramadan/remote-keylogger/assets/155490852/6e0bbd96-9fb8-4f27-9418-2d8a1ff24260)

### Host Information and WiFi Profiles:
Utilized functions to collect host information and saved WiFi profiles, providing comprehensive details about the host machine.

![image](https://github.com/moeramadan/remote-keylogger/assets/155490852/be013642-c620-46a3-a52e-6e1fad777d38)

### Main Loop:
Implemented the main functions and loop to continuously capture keystrokes, write them to a temporary file, and send the data remotely via email. Included functionality to terminate the program using a safety key.

![image](https://github.com/moeramadan/remote-keylogger/assets/155490852/ffe7a11a-c537-4cb2-90ad-ef14735f7606)
![image](https://github.com/moeramadan/remote-keylogger/assets/155490852/e4cdd37f-822d-4351-8f74-76dc330fd4c9)

## Executable Compilation:
Utilizing PyInstaller via the command line, the Python program can seamlessly transform into a standalone executable. By employing the ".pyw" extension, the program operates in a mode devoid of any console presence, ensuring inconspicuous execution without triggering command prompts or new windows.

![image](https://github.com/moeramadan/remote-keylogger/assets/155490852/4bfe2b58-f249-4cef-ad09-f2fd09f704f7)


## WinRAR Packaging:
Leveraging WinRAR, we orchestrate the bundling of files into a Self-Extracting (SFX) archive. This ingenious method involves embedding the program within an innocuous image file, thus executing the keylogger covertly upon opening. While adeptly concealing the icon and file opening behavior, the file type remains indistinguishable from a standard application.

![image](https://github.com/moeramadan/remote-keylogger/assets/155490852/3a49e736-5665-42b4-838f-1016d8c6e127)


## Demo:
Upon initiating the disguised image file, the executable seamlessly launches, initiating the process of transmitting host information and keystrokes via email. This operation persists until the user intervenes by pressing the right Ctrl key, thereby terminating the program discreetly.

![image](https://github.com/moeramadan/remote-keylogger/assets/155490852/5875d9f0-3e92-4d9b-b71b-57df81940bfc)
![image](https://github.com/moeramadan/remote-keylogger/assets/155490852/9c3311ce-ba7f-4237-af9d-1ba17dbd8c47)
![image](https://github.com/moeramadan/remote-keylogger/assets/155490852/2563efcb-9b64-4dd0-b5c1-5b454762e295)



