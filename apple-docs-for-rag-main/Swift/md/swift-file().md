

- Swift
-  file() 

Macro

# file()

Produces the path to the file in which it appears.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@freestanding(expression)
macro file() -> T where T : ExpressibleByStringLiteral
```

## Overview

The string value from `#file` depends on the language version, to enable migration from the old `#filePath` behavior to the new `#fileID` behavior. Currently, `#file` has the same value as `#filePath`. In a future version of Swift, `#file` will have the same value as `#fileID` instead. To adopt the future behavior, replace `#file` with `#fileID` or `#filePath` as appropriate.

This macro’s value can be changed by `#sourceLocation`, as described in Line Control Statement in *The Swift Programming Language*.

## See Also

### Getting Source Location Information

macro fileID&lt;T>() -> T

Produces a unique identifier for the source file in which the macro appears.

macro filePath&lt;T>() -> T

Produces the complete path to the file in which the macro appears.

macro function&lt;T>() -> T

Produces the name of the declaration in which it appears.

macro line&lt;T>() -> T

Produces the line number on which it appears.

macro column&lt;T>() -> T

Produces the column number in which the macro begins.

