

- Swift
-  fileID() 

Macro

# fileID()

Produces a unique identifier for the source file in which the macro appears.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@freestanding(expression)
macro fileID() -> T where T : ExpressibleByStringLiteral
```

## Overview

The unique identifier has the form *module*/*file*, where *file* is the name of the file in which the expression appears and *module* is the name of the module that this file is part of.

Because `#fileID` doesn’t embed the full path to the source file, unlike `#filePath`, it gives you better privacy and reduces the size of the compiled binary.

Note: To parse a `#fileID` expression, read the module name as the text before the first slash (`/`) and the filename as the text after the last slash. In future versions of Swift, the string might contain multiple slashes, such as `MyModule/some/disambiguation/MyFile.swift`.

This macro’s value can be changed by `#sourceLocation`, as described in Line Control Statement in *The Swift Programming Language*.

## See Also

### Getting Source Location Information

macro file&lt;T>() -> T

Produces the path to the file in which it appears.

macro filePath&lt;T>() -> T

Produces the complete path to the file in which the macro appears.

macro function&lt;T>() -> T

Produces the name of the declaration in which it appears.

macro line&lt;T>() -> T

Produces the line number on which it appears.

macro column&lt;T>() -> T

Produces the column number in which the macro begins.

