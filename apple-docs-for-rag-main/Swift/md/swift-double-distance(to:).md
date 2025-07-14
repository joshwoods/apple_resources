

- Swift
- Double
-  distance(to:) 

Instance Method

# distance(to:)

Returns the distance from this value to the given value, expressed as a stride.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func distance(to other: Double) -> Double
```

## Parameters 

`other`  

The value to calculate the distance to.

## Return Value

The distance from this value to `other`.

## Discussion

If this type’s `Stride` type conforms to `BinaryInteger`, then for two values `x` and `y`, and a distance `n = x.distance(to: y)`, `x.advanced(by: n) == y`. Using this method with types that have a noninteger `Stride` may result in an approximation.

Complexity

O(1)

## See Also

### Infrequently Used Functionality

init()

init(floatLiteral: Double)

Creates an instance initialized to the specified floating-point value.

init(integerLiteral: Int64)

Creates an instance initialized to the specified integer value.

init(integerLiteral: Self)

typealias FloatLiteralType

A type that represents a floating-point literal.

typealias IntegerLiteralType

A type that represents an integer literal.

func advanced(by: Double) -> Double

Returns a value that is offset the specified distance from this value.

typealias Stride

A type that represents the distance between two values.

func write&lt;Target>(to: inout Target)

Writes a textual representation of this instance into the given output stream.

var hashValue: Int

The hash value.

