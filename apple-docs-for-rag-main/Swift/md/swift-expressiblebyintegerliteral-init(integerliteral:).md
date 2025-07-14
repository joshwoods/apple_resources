

- Swift
- ExpressibleByIntegerLiteral
-  init(integerLiteral:) 

Initializer

# init(integerLiteral:)

Creates an instance initialized to the specified integer value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(integerLiteral value: Self.IntegerLiteralType)
```

**Required** Default implementation provided.

## Parameters 

`value`  

The value to create.

## Discussion

Do not call this initializer directly. Instead, initialize a variable or constant using an integer literal. For example:

```
let x = 23
```

In this example, the assignment to the `x` constant calls this integer literal initializer behind the scenes.

## Default Implementations

### ExpressibleByIntegerLiteral Implementations

init(integerLiteral: Self)

