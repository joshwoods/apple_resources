

- Swift
-  warning(\_:) 

Macro

# warning(\_:)

Produces the given warning message during compilation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@freestanding(declaration)
macro warning(_ message: String)
```

## Parameters 

`warning`  

The diagnostic message.

## Overview

Compilation proceeds after emitting the message as a nonfatal warning.

## See Also

### Generating Compile-Time Diagnostics

macro error(String)

Emits the given message as a fatal error and terminates the compilation process.

