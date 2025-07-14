

- Swift
-  CommandLine 

Enumeration

# CommandLine

Command-line arguments for the current process.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum CommandLine
```

## Topics

### Accessing Arguments

static var arguments: [String]

An array that provides access to this program’s command line arguments.

### Accessing Raw Argument Data

static var argc: Int32

Access to the raw argc value from C.

static var unsafeArgv: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;Int8>?>

Access to the raw argv value from C.

## Relationships

### Conforms To

- Sendable

## See Also

### Command Line Input

func readLine(strippingNewline: Bool) -> String?

Returns a string read from standard input through the end of the current line or until EOF is reached.

