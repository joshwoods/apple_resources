

- Swift
- Double
-  advanced(by:) 

Instance Method

# advanced(by:)

Returns a value that is offset the specified distance from this value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func advanced(by amount: Double) -> Double
```

## Return Value

A value that is offset from this value by `n`.

## Discussion

Use the `advanced(by:)` method in generic code to offset a value by a specified distance. If you’re working directly with numeric values, use the addition operator (`+`) instead of this method.

```
func addOne(to x: T) -> T
    where T.Stride: ExpressibleByIntegerLiteral
{
    return x.advanced(by: 1)
}

let x = addOne(to: 5)
// x == 6
let y = addOne(to: 3.5)
// y = 4.5
```

If this type’s `Stride` type conforms to `BinaryInteger`, then for a value `x`, a distance `n`, and a value `y = x.advanced(by: n)`, `x.distance(to: y) == n`. Using this method with types that have a noninteger `Stride` may result in an approximation. If the result of advancing by `n` is not representable as a value of this type, then a runtime error may occur.

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

func distance(to: Double) -> Double

Returns the distance from this value to the given value, expressed as a stride.

typealias Stride

A type that represents the distance between two values.

func write&lt;Target>(to: inout Target)

Writes a textual representation of this instance into the given output stream.

var hashValue: Int

The hash value.

