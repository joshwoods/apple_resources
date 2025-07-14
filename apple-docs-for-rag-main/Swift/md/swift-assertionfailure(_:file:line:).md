

- Swift
-  assertionFailure(\_:file:line:) 

Function

# assertionFailure(\_:file:line:)

Indicates that an internal consistency check failed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func assertionFailure(
    _ message: @autoclosure () -> String = String(),
    file: StaticString = #file,
    line: UInt = #line
)
```

## Parameters 

`message`  

A string to print in a playground or `-Onone` build. The default is an empty string.

`file`  

The file name to print with `message`. The default is the file where `assertionFailure(_:file:line:)` is called.

`line`  

The line number to print along with `message`. The default is the line number where `assertionFailure(_:file:line:)` is called.

## Discussion

This function’s effect varies depending on the build flag used:

- In playgrounds and `-Onone` builds (the default for Xcode’s Debug configuration), stop program execution in a debuggable state after printing `message`.

- In `-O` builds, has no effect.

- In `-Ounchecked` builds, the optimizer may assume that this function is never called. Failure to satisfy that assumption is a serious programming error.

## See Also

### Testing

func assert(@autoclosure () -> Bool, @autoclosure () -> String, file: StaticString, line: UInt)

Performs a traditional C-style assert with an optional message.

func precondition(@autoclosure () -> Bool, @autoclosure () -> String, file: StaticString, line: UInt)

Checks a necessary condition for making forward progress.

func preconditionFailure(@autoclosure () -> String, file: StaticString, line: UInt) -> Never

Indicates that a precondition was violated.

