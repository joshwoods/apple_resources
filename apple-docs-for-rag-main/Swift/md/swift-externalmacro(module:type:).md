

- Swift
-  externalMacro(module:type:) 

Macro

# externalMacro(module:type:)

Specifies the module and type name for a macro’s implementation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@freestanding(expression)
macro externalMacro(
    module: String,
    type: String
) -> T
```

## Parameters 

`module`  

The module name.

`type`  

The type that implements the macro.

## Return Value

The macro’s implementation.

## Overview

This macro can only be used to define a macro; using it in any other context is an error. The specified type must conform to the protocols that correspond to the roles of the macro being declared. For example:

```
macro stringify(_ value: T) -> (T, String) =
    #externalMacro(module: "ExampleMacros", type: "StringifyMacro")
```

