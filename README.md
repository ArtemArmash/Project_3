```markdown
# Simple C++ Struct Example

This is a basic C++ console application that demonstrates the use of structs, header files, and simple user input/output. The program prompts the user to enter their name and age, and then displays the entered information back to the console.

## About The Project

This project was created to illustrate fundamental C++ concepts in a clear and organized way. It is a great starting point for beginners who are learning about:

*   **Data Structuring**: Using `struct` to group related data (`Human`).
*   **Code Organization**: Splitting code into multiple files (`.h` headers and a `.cpp` source file) for better readability and management.
*   **Console I/O**: Interacting with the user via the console using `std::cin` and `std::cout`.
*   **Header Guards**: Using `#pragma once` to prevent multiple inclusions of header files.

## Project Structure

The code is divided into three main files:

*   `Human.h`: Defines the `Human` struct, which holds data for a person (name and age) and a method to display this data.
*   `StartAp.h`: Defines the `StartUp` struct, which orchestrates the application flow. It contains methods for getting user input and starting the main logic.
*   `ConsoleApplication158.cpp`: The main entry point of the application. It creates an instance of the `StartUp` struct and runs it.

## Getting Started

To compile and run this project, you need a C++ compiler (like G++, Clang, or MSVC).

### How to Build

1.  Make sure all three files (`Human.h`, `StartAp.h`, `ConsoleApplication158.cpp`) are in the same directory.
2.  Open a terminal or command prompt in that directory.
3.  Compile the project using your C++ compiler. For example, with g++:
    ```sh
    g++ ConsoleApplication158.cpp -o user_app
    ```
4.  Run the compiled executable:
    ```sh
    ./user_app
    ```
    On Windows, you would run:
    ```cmd
    user_app.exe
    ```

## Usage

When you run the application, it will prompt you to enter your name and age.

```
Enter your name & age:      
```

First, type your full name and press `Enter`. Then, type your age and press `Enter` again. The program will then display the information you provided.

**Example Session:**

```
Enter your name & age: John Doe
42
John Doe
42
```

**Note:** There is a known issue in the `Input` function where `cin >> human.age` can leave a newline character in the input buffer, which might cause problems in more complex programs. For this simple example, it works as expected.
```

