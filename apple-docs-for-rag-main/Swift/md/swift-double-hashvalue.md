

- Swift
- Double
-  hashValue 

Instance Property

# hashValue

The hash value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var hashValue: Int { get }
```

## Discussion

Hash values are not guaranteed to be equal across different executions of your program. Do not save hash values to use during a future execution.

Important

`hashValue` is deprecated as a `Hashable` requirement. To conform to `Hashable`, implement the `hash(into:)` requirement instead. The compiler provides an implementation for `hashValue` for you.

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

func distance(to: Double) -> Double

Returns the distance from this value to the given value, expressed as a stride.

typealias Stride

A type that represents the distance between two values.

func write&lt;Target>(to: inout Target)

Writes a textual representation of this instance into the given output stream.

