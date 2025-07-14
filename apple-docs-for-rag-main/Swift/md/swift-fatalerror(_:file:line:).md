

- Swift
-  fatalError(\_:file:line:) 

Function

# fatalError(\_:file:line:)

Unconditionally prints a given message and stops execution.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func fatalError(
    _ message: @autoclosure () -> String = String(),
    file: StaticString = #file,
    line: UInt = #line
) -> Never
```

## Parameters 

`message`  

The string to print. The default is an empty string.

`file`  

The file name to print with `message`. The default is the file where `fatalError(_:file:line:)` is called.

`line`  

The line number to print along with `message`. The default is the line number where `fatalError(_:file:line:)` is called.

## See Also

### Exiting a Program

enum Never

A type that has no values and can’t be constructed.

