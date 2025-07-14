

- Swift
-  function() 

Macro

# function()

Produces the name of the declaration in which it appears.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@freestanding(expression)
macro function() -> T where T : ExpressibleByStringLiteral
```

## Overview

Inside a function, the value `#function` produces is the name of that function, inside a method it’s the name of that method, inside a property getter or setter it’s the name of that property, inside special members like `init` or `subscript` it’s the name of that keyword, and at the top level of a file it’s the name of the current module.

When used as the default value of a function or method parameter, this macro’s value is determined when the default value expression is evaluated at the call site. For example:

```
func logFunctionName(string: String = #function) {
    print(string)
}
func myFunction() {
    logFunctionName() // Prints "myFunction()".
}
```

## See Also

### Getting Source Location Information

macro file&lt;T>() -> T

Produces the path to the file in which it appears.

macro fileID&lt;T>() -> T

Produces a unique identifier for the source file in which the macro appears.

macro filePath&lt;T>() -> T

Produces the complete path to the file in which the macro appears.

macro line&lt;T>() -> T

Produces the line number on which it appears.

macro column&lt;T>() -> T

Produces the column number in which the macro begins.

