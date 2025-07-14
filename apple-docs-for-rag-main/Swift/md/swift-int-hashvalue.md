

- Swift
- Int
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

Creates a new value equal to zero.

init(integerLiteral: Self)

typealias IntegerLiteralType

A type that represents an integer literal.

func distance(to: Int) -> Int

Returns the distance from this value to the given value, expressed as a stride.

func advanced(by: Int) -> Int

Returns a value that is offset the specified distance from this value.

typealias Stride

A type that represents the distance between two values.

