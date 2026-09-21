# PLP 1: Getting Started with Dart

## 1. History and Background

### When, Where, and Why Was Dart Created?

Dart was developed at Google by Lars Bak and Kasper Lund and first introduced in October 2011 at the GOTO conference in Aarhus, Denmark.

Source: [Dart — Wikipedia](https://en.wikipedia.org/wiki/Dart_%28programming_language%29)

It was created to meet the need for a structured but flexible language for web development. Its original goals were to be familiar and easy for programmers to learn, while providing high performance across modern browsers and environments ranging from mobile devices to servers.

Source: [Dart: A Language for Structured Web Programming — Lars Bak, Google Developers Blog](https://developers.googleblog.com/dart-a-language-for-structured-web-programming/)

### What Is Dart Used For?

Dart is mainly used to build mobile, web, and desktop applications. It can also be used for command-line tools and server applications.

Sources: [Dart Overview](https://dart.dev/overview), [Dart SDK](https://dart.dev/get-dart)

Examples of applications developed using Dart with the Flutter framework include Google Pay and the My BMW app, which connects drivers with their vehicles.

Sources: [Google Pay — Flutter Case Study](https://flutter.dev/showcase/google-pay), [BMW — Flutter Case Study](https://flutter.dev/showcase/bmw)

### What Is Flutter, and How Is It Related to Dart?

Flutter is a framework for building mobile, web, and desktop applications using Dart. Dart is the programming language used to write application code, while Flutter provides tools and widgets for creating the user interface, such as buttons, text fields, and screens.

Source: [Dart Overview](https://dart.dev/overview)

### Where Will I Learn Dart?

When I start programming in Dart, I will use the tutorial on the official Dart website, the Dart tutorial on GeeksforGeeks, and a YouTube tutorial playlist to learn the basics and find coding examples.

1. [Dart’s official tutorial](https://dart.dev/learn/tutorial)
2. [GeeksforGeeks Dart tutorial](https://www.geeksforgeeks.org/dart/dart-tutorial/)
3. [YouTube tutorial playlist](https://www.youtube.com/playlist?list=PLptHs0ZDJKt_fLp8ImPQVc1obUJKDSQL7)



## 2. Installation and Programming Environment

### Installing the Dart SDK

To write and run Dart programs, I installed the Dart SDK on Windows. The SDK includes the libraries and command-line tools needed to develop Dart programs.

Follow these steps to install it:

1. Open the [Dart SDK download page](https://dart.dev/get-dart/archive).
2. Select the stable release, choose Windows, and select the architecture that matches your computer. I used x64.
3. Download and extract the ZIP file.
4. Find the `bin` folder inside the extracted `dart-sdk` folder. On my computer, the path is: `S:\dartsdk-windows-x64-release\dart-sdk\bin`

5. In Windows Search, search for **Edit environment variables for your account**.
6. Under **User variables**, select **Path**, click **Edit**, and then click **New**.
7. Add the path to your Dart SDK’s `bin` folder. Use your own path if you extracted the SDK somewhere else.
8. Save the changes and restart any open terminals and VS Code.

Adding the `bin` folder to Path allows Windows to find the `dart` command without requiring its full location.

Open PowerShell or a terminal in VS Code and run:

```powershell
dart --version
```

My installation reported Dart SDK version **3.13.4 (stable)**. Your version may be different.

If the terminal says that `dart` is not recognized, check that the Path entry points to the folder containing `dart.exe`, then close and reopen the terminal.

Source: [Get the Dart SDK](https://dart.dev/get-dart)

### Choosing and Setting Up Visual Studio Code

Dart does not require one specific programming environment. Its official documentation provides setup instructions for Visual Studio Code with the Dart extension.

I chose Visual Studio Code because I can edit my code and run commands in its built-in terminal. The Dart extension adds language support, such as syntax highlighting.

To set it up:

1. Download and install [Visual Studio Code](https://code.visualstudio.com/) if it is not already installed.
2. Open VS Code and press **Ctrl + Shift + X** to open the Extensions panel.
3. Search for **Dart** and install the extension published by **Dart Code**.
4. Select **File → Open Folder** and open the folder where you want to save your Dart programs.
5. Select **Terminal → New Terminal** to open a terminal inside VS Code.

The Dart extension supports writing code in the editor, while the Dart SDK provides the tools that run the program. Both are needed for the setup described here.

Source: [Visual Studio Code — Dart Documentation](https://dart.dev/tools/vs-code)



## 3. Running a Dart Program

### Hello World Example

### How to Run the Program



## 4. Comments in Dart

### Single-Line Comments

### Multi-Line Comments

### Documentation Comments



## 5. Resources
