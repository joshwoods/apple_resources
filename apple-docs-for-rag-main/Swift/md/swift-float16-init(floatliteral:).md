

- Swift
- Float16
-  init(floatLiteral:) 

Initializer

# init(floatLiteral:)

Creates an instance initialized to the specified floating-point value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(floatLiteral value: Float16)
```

## Parameters 

`value`  

The value to create.

## Discussion

Do not call this initializer directly. Instead, initialize a variable or constant using a floating-point literal. For example:

```
let x = 21.5
```

In this example, the assignment to the `x` constant calls this floating-point literal initializer behind the scenes.

