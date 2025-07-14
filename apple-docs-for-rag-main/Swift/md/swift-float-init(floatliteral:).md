

- Swift
- Float
-  init(floatLiteral:) 

Initializer

# init(floatLiteral:)

Creates an instance initialized to the specified floating-point value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(floatLiteral value: Float)
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

## See Also

### Infrequently Used Functionality

init()

init(integerLiteral: Int64)

Creates an instance initialized to the specified integer value.

init(integerLiteral: Self)

func advanced(by: Float) -> Float

Returns a value that is offset the specified distance from this value.

func distance(to: Float) -> Float

Returns the distance from this value to the given value, expressed as a stride.

func write&lt;Target>(to: inout Target)

Writes a textual representation of this instance into the given output stream.

