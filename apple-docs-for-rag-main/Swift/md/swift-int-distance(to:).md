

- Swift
- Int
-  distance(to:) 

Instance Method

# distance(to:)

Returns the distance from this value to the given value, expressed as a stride.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func distance(to other: Int) -> Int
```

## Parameters 

`other`  

The value to calculate the distance to.

## Return Value

The distance from this value to `other`.

## Discussion

For two values `x` and `y`, and a distance `n = x.distance(to: y)`, `x.advanced(by: n) == y`.

## See Also

### Infrequently Used Functionality

init()

Creates a new value equal to zero.

init(integerLiteral: Self)

typealias IntegerLiteralType

A type that represents an integer literal.

func advanced(by: Int) -> Int

Returns a value that is offset the specified distance from this value.

typealias Stride

A type that represents the distance between two values.

var hashValue: Int

The hash value.

