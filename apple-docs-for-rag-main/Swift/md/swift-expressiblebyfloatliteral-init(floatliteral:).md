

- Swift
- ExpressibleByFloatLiteral
-  init(floatLiteral:) 

Initializer

# init(floatLiteral:)

Creates an instance initialized to the specified floating-point value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(floatLiteral value: Self.FloatLiteralType)
```

**Required**

## Parameters 

`value`  

The value to create.

## Discussion

Do not call this initializer directly. Instead, initialize a variable or constant using a floating-point literal. For example:

```
let x = 21.5
```

In this example, the assignment to the `x` constant calls this floating-point literal initializer behind the scenes.

