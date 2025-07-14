

- Swift
- Float16
-  init(integerLiteral:) 

Initializer

# init(integerLiteral:)

Creates an instance initialized to the specified integer value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(integerLiteral value: Int64)
```

## Parameters 

`value`  

The value to create.

## Discussion

Do not call this initializer directly. Instead, initialize a variable or constant using an integer literal. For example:

```
let x = 23
```

In this example, the assignment to the `x` constant calls this integer literal initializer behind the scenes.

