# Dart Overview and Setup

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

The SDK includes the libraries and command-line tools needed to develop Dart programs. The official Dart website lists several installation methods, including downloading the SDK as a ZIP file. I used the ZIP method on Windows. The steps below describe the installation process I followed on my computer.

Official installation information: [Get the Dart SDK](https://dart.dev/get-dart)

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

### Choosing and Setting Up Visual Studio Code

The official Dart website presents DartPad as an easy way to learn Dart syntax and experiment with the language without downloading any software. DartPad runs directly in a web browser. Dart also supports development in editors such as Visual Studio Code.

Sources: [Dart Development Tools](https://dart.dev/tools), [DartPad](https://dart.dev/tools/dartpad)

I chose Visual Studio Code because it was already installed on my computer, and I was relatively familiar with it. I also knew that VS Code supports Dart through an extension, so it was a convenient choice for me.

To set up VS Code for Dart:

1. Download and install [Visual Studio Code](https://code.visualstudio.com/) if it is not already installed.
2. Open VS Code and press **Ctrl + Shift + X** to open the Extensions panel.
3. Search for **Dart** and install the extension published by **Dart Code**.
4. Select **File → Open Folder** and open the folder where you want to save your Dart programs.
5. Select **Terminal → New Terminal** to open a terminal inside VS Code.

The Dart extension adds support for working with Dart code in the editor. To run programs locally, install the Dart SDK as described in the previous section.

Source: [Visual Studio Code — Dart Documentation](https://dart.dev/tools/vs-code)


## 3. Running a Dart Program

### Hello World Example

Example source code: [Hello World](Hello%20World.dart)

In VS Code, open your project folder and create a file named `main.dart`. Add the following code and save the file:

```dart
void main() {
  print('Hello, world!');
}
```

The `main()` function is where the program starts. The `void` keyword means that the function does not return a value. The `print()` function displays the message in the terminal.

### How to Run the Program

Open **Terminal → New Terminal** in VS Code. Make sure the terminal is in the folder containing `main.dart`.

On my computer, the terminal prompt looks like this: `PS S:\CS 330\PLP>`

This prompt shows that the terminal is already in my project folder. You do not need to type the prompt yourself.

Run the program with:

```powershell
dart run main.dart
```

The `dart run` command runs the Dart file you specify. This example does not require any additional packages.

The expected output is: `hello world`

After changing the code, save the file and run the same command again to see the updated output.

Source: [Dart Run — Dart Documentation](https://dart.dev/tools/dart-run)



## 4. Comments in Dart

Comments explain what the code does without changing how the program runs. Dart supports single-line comments, multi-line comments, and documentation comments.

### Single-Line Comments

A single-line comment starts with `//`. Everything after `//` on that line is treated as a comment.

```dart
void main() {
  // Display the greeting.
  print('hello world');
}
```

A comment can also appear after a statement:

```dart
void main() {
  print('hello world'); // Display the greeting.
}
```

### Multi-Line Comments

A multi-line comment starts with `/*` and ends with `*/`. It can be used for explanations that take more than one line.

```dart
/*
Display the greeting.
*/
void main() {
  print('hello world');
}
```

Dart also allows multi-line comments to be nested inside other multi-line comments.

### Documentation Comments

Documentation comments describe functions, classes, and other parts of a program. They start with `///` or use the block form `/** ... */`.

Place a documentation comment immediately before the item it describes:

```dart
/// Display the greeting.
/// Display the greeting.
/// Display the greeting.

/**
 * Display the greeting.
 * Display the greeting.
 */

void main() {
  print('hello world');
}
```

Source: [Comments — Dart Documentation](https://dart.dev/language/comments)

## 5. Resources

### References and Tools

1. [Dart — Wikipedia](https://en.wikipedia.org/wiki/Dart_%28programming_language%29)
2. [Dart: A Language for Structured Web Programming — Lars Bak, Google Developers Blog](https://developers.googleblog.com/dart-a-language-for-structured-web-programming/)
3. [Dart Overview](https://dart.dev/overview)
4. [Google Pay — Flutter Case Study](https://flutter.dev/showcase/google-pay)
5. [BMW — Flutter Case Study](https://flutter.dev/showcase/bmw)
6. [Get the Dart SDK](https://dart.dev/get-dart)
7. [Dart SDK Archive](https://dart.dev/get-dart/archive)
8. [Dart Development Tools](https://dart.dev/tools)
9. [DartPad — Dart Documentation](https://dart.dev/tools/dartpad)
10. [Visual Studio Code — Official Website](https://code.visualstudio.com/)
11. [Visual Studio Code — Dart Documentation](https://dart.dev/tools/vs-code)
12. [Dart Run — Dart Documentation](https://dart.dev/tools/dart-run)
13. [Comments — Dart Documentation](https://dart.dev/language/comments)

### Learning Resources

I plan to use the following resources to learn Dart and find coding examples:

1. [Dart’s Official Tutorial](https://dart.dev/learn/tutorial)
2. [GeeksforGeeks Dart Tutorial](https://www.geeksforgeeks.org/dart/dart-tutorial/)
3. [YouTube Tutorial Playlist](https://www.youtube.com/playlist?list=PLptHs0ZDJKt_fLp8ImPQVc1obUJKDSQL7)
