# My Shelfie – Software Engineering Project 2022/2023
## 👥 Team Members
* [Alessandro Mancini](https://github.com/alemancio5)
* [Chiara Thien Thao Nguyen Ba](https://github.com/chiaranb)
* [Flavia Nicotri](https://github.com/flanico)
* [Stefano Morano](https://github.com/stefano-morano)

## Project Overview

**MyShelfie** is a strategy board game where players compete to organize their bookshelf in the most efficient way possible.

This project is a digital implementation of the board game, featuring:
- A multiplayer architecture supporting both **Socket** and **RMI** communication.
- Two client interfaces: **CLI** (Command-Line) and **GUI** (Graphical).
- Complete implementation of game rules, game state persistence, and chat functionality.

📖 [Official Game Rules](https://www.craniocreations.it/prodotto/my-shelfie)


## Features

| Feature              | Status |
|----------------------|:------:|
| Simplified Rules     | ✅      |
| Complete Rules       | ✅      |
| Socket Support       | ✅      |
| RMI Support          | ✅      |
| CLI Interface        | ✅      |
| GUI Interface        | ✅      |
| Chat System          | ✅      |
| Game State Persistence | ✅   |
| Fault Tolerance      | ❌      |
| Multiple Concurrent Games | ❌ |

---

## How to Run

> **Requirements**: Java 19 or higher installed on your system.

### Starting the Server
To launch the server, open a terminal in the folder containing the JAR file and run:

```java -jar ServerApp.jar```

You will then be prompted to enter two port numbers for Socket and RMI communication.
Press Enter to use the default ports.
Once the message "server is running" appears, the server is ready to accept connections.

### Starting the Client
To launch the client, open a terminal in the folder containing the JAR file and run:

```java -jar ClientApp.jar```

You’ll be asked to choose the interface:
	•	Enter c for the Command-Line Interface (CLI)
	•	Enter g for the Graphical User Interface (GUI)

#### CLI Mode
- First, choose the connection type:
- Enter s for Socket or r for RMI
- Then, enter the server’s IP address and port
(Press Enter to use the default values)

#### GUI Mode
On the connection screen, click the “Continue” button without modifying any fields to connect to the server using the default Socket/RMI ports.

## Tools Used
* [IntelliJ IDEA](https://www.jetbrains.com/idea/) -  IDE used for development
* [Maven](https://maven.apache.org/) - Dependency Management
* [JavaFX](https://openjfx.io/) - Graphical User Interface (GUI) 
* [Scene Builder](https://gluonhq.com/products/scene-builder/) - GUI layout design 
* [draw.io](https://app.diagrams.net/) - UML and Sequence diagrams

## Q&A
###  How can I see the effect of the Common Goal cards in the GUI?
Click on a Common Goal card with the mouse to view its effect.
### What if CLI colors are not displayed correctly?
If colors in the CLI don’t display properly on Windows, open CMD as Administrator and run the following command:

```REG ADD HKCU\CONSOLE /f /v VirtualTerminalLevel /t REG_DWORD /d 1```
###  What if my system’s Java version isn’t compatible?
You must install Java version 19 or higher to run the program correctly.
You can download it from the official Java website [link](https://www.oracle.com/it/java/technologies/downloads/).
