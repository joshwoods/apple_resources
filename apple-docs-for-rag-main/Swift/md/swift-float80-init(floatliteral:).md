

- Swift
- Float80
-  init(floatLiteral:) 

Initializer

# init(floatLiteral:)

Creates an instance initialized to the specified floating-point value.

macOS 10.10+

``` source
init(floatLiteral value: Float80)
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

