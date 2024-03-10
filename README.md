# Simple Notes App

This simple notes application is built in Go and demonstrates basic programming concepts, including creating, displaying, and saving notes. Below are the key concepts and Go features utilized in this application.

## Key Concepts

### Custom Package Creation and Usage
- The application is divided into two main parts: the main application logic and the `note` package.
- The `note` package encapsulates the functionality related to a note, such as creation, display, and saving.

### Structs and Methods
- A `Note` struct is defined in the `note` package, holding the note's title, content, and creation date.
- Methods on the `Note` struct (`Display` and `Save`) provide functionality to display the note's content and save the note to a file, respectively.

### Error Handling
- Error handling is prominently used throughout the application, especially in creating a new note and saving a note to a file, to ensure robustness.

### File I/O
- The application demonstrates file input/output operations by saving notes in JSON format to the local file system, using `os.WriteFile` and `json.Marshal`.

### Standard Library Utilization
- Utilizes the `bufio`, `fmt`, `os`, `strings`, `time`, and `encoding/json` packages from Go's standard library for various functionalities like reading user input, string manipulation, JSON processing, and handling date and time.

### User Input
- Collects user input for the note's title and content using the `bufio` reader and `os.Stdin`, showcasing basic user interaction through the console.

### JSON Encoding
- Converts the note into JSON format using `json.Marshal`, demonstrating how to work with JSON in Go, including adding struct tags to customize the JSON keys.

## Getting Started

To run this application, ensure you have Go installed on your system. Clone the repository, navigate to the project directory, and run:

```sh
go run .
```
