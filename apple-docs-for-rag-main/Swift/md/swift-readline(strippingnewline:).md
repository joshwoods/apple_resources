

- Swift
-  readLine(strippingNewline:) 

Function

# readLine(strippingNewline:)

Returns a string read from standard input through the end of the current line or until EOF is reached.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func readLine(strippingNewline: Bool = true) -> String?
```

## Parameters 

`strippingNewline`  

If `true`, newline characters and character combinations are stripped from the result; otherwise, newline characters or character combinations are preserved. The default is `true`.

## Return Value

The string of characters read from standard input. If EOF has already been reached when `readLine()` is called, the result is `nil`.

## Discussion

Standard input is interpreted as `UTF-8`. Invalid bytes are replaced by Unicode replacement characters.

## See Also

### Command Line Input

enum CommandLine

Command-line arguments for the current process.

