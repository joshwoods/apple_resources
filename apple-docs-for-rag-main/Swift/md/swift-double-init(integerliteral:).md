

- Swift
- Double
-  init(integerLiteral:) 

Initializer

# init(integerLiteral:)

Creates an instance initialized to the specified integer value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

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

## See Also

### Infrequently Used Functionality

init()

init(floatLiteral: Double)

Creates an instance initialized to the specified floating-point value.

init(integerLiteral: Self)

typealias FloatLiteralType

A type that represents a floating-point literal.

typealias IntegerLiteralType

A type that represents an integer literal.

func advanced(by: Double) -> Double

Returns a value that is offset the specified distance from this value.

func distance(to: Double) -> Double

Returns the distance from this value to the given value, expressed as a stride.

typealias Stride

A type that represents the distance between two values.

func write&lt;Target>(to: inout Target)

Writes a textual representation of this instance into the given output stream.

var hashValue: Int

The hash value.

