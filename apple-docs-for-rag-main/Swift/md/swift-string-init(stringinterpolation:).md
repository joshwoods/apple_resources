

- Swift
- String
-  init(stringInterpolation:) 

Initializer

# init(stringInterpolation:)

Creates a new instance from an interpolated string literal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(stringInterpolation: DefaultStringInterpolation)
```

## Discussion

Do not call this initializer directly. It is used by the compiler when you create a string using string interpolation. Instead, use string interpolation to create a new string by including values, literals, variables, or expressions enclosed in parentheses, prefixed by a backslash (`\(`…`)`).

```
let price = 2
let number = 3
let message = """
              If one cookie costs \(price) dollars, \
              \(number) cookies cost \(price * number) dollars.
              """
print(message)
// Prints "If one cookie costs 2 dollars, 3 cookies cost 6 dollars."
```

## See Also

### Infrequently Used Functionality

func index(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

init(NSString)

init(stringLiteral: String)

Creates an instance initialized to the given string value.

init(unicodeScalarLiteral: Self.ExtendedGraphemeClusterLiteralType)

init(extendedGraphemeClusterLiteral: Self.StringLiteralType)

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for the `String` instance.

Deprecated

func withContiguousStorageIfAvailable&lt;R>((UnsafeBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R?

Executes a closure on the sequence’s contiguous storage.

