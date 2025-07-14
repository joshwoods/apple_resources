

- Swift
- Double
-  Double.FloatLiteralType 

Type Alias

# Double.FloatLiteralType

A type that represents a floating-point literal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias FloatLiteralType = Double
```

## Discussion

Valid types for `FloatLiteralType` are `Float`, `Double`, and `Float80` where available.

## See Also

### Infrequently Used Functionality

init()

init(floatLiteral: Double)

Creates an instance initialized to the specified floating-point value.

init(integerLiteral: Int64)

Creates an instance initialized to the specified integer value.

init(integerLiteral: Self)

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

