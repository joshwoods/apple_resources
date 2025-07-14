

- Swift
- String
-  init(stringLiteral:) 

Initializer

# init(stringLiteral:)

Creates an instance initialized to the given string value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(stringLiteral value: String)
```

## Discussion

Do not call this initializer directly. It is used by the compiler when you initialize a string using a string literal. For example:

```
let nextStop = "Clark & Lake"
```

This assignment to the `nextStop` constant calls this string literal initializer behind the scenes.

## See Also

### Infrequently Used Functionality

func index(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

init(NSString)

init(stringInterpolation: DefaultStringInterpolation)

Creates a new instance from an interpolated string literal.

init(unicodeScalarLiteral: Self.ExtendedGraphemeClusterLiteralType)

init(extendedGraphemeClusterLiteral: Self.StringLiteralType)

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for the `String` instance.

Deprecated

func withContiguousStorageIfAvailable&lt;R>((UnsafeBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R?

Executes a closure on the sequence’s contiguous storage.

