

- Swift
- Float80
-  init(integerLiteral:) 

Initializer

# init(integerLiteral:)

Creates an instance initialized to the specified integer value.

macOS 10.10+

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

