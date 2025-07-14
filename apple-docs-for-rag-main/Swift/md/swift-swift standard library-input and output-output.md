

- Swift
- Swift Standard Library
-  Input and Output 

API Collection

# Input and Output

Print values to the console, read from and write to text streams, and use command line arguments.

## Topics

### Text Output

func print(Any..., separator: String, terminator: String)

Writes the textual representations of the given items into the standard output.

func print&lt;Target>(Any..., separator: String, terminator: String, to: inout Target)

Writes the textual representations of the given items into the given output stream.

### Command Line Input

enum CommandLine

Command-line arguments for the current process.

func readLine(strippingNewline: Bool) -> String?

Returns a string read from standard input through the end of the current line or until EOF is reached.

### Streams

protocol TextOutputStream

A type that can be the target of text-streaming operations.

protocol TextOutputStreamable

A source of text-streaming operations.

## See Also

### Programming Tasks

Debugging and Reflection

Fortify your code with runtime checks, and examine your values’ runtime representation.

Macros

Generate boilerplate code and perform other compile-time operations.

Concurrency

Perform asynchronous and parallel operations.

Key-Path Expressions

Use key-path expressions to access properties dynamically.

Manual Memory Management

Allocate and manage memory manually.

Type Casting and Existential Types

Perform casts between types or represent values of any type.

C Interoperability

Use imported C types or call C variadic functions.

Operator Declarations

Work with prefix, postfix, and infix operators.

