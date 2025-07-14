

- Swift
- String
-  init(unicodeScalarLiteral:) 

Initializer

# init(unicodeScalarLiteral:)

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(unicodeScalarLiteral value: Self.ExtendedGraphemeClusterLiteralType)
```

Available when `ExtendedGraphemeClusterLiteralType` is `Self.UnicodeScalarLiteralType`.

## See Also

### Infrequently Used Functionality

func index(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

init(NSString)

init(stringInterpolation: DefaultStringInterpolation)

Creates a new instance from an interpolated string literal.

init(stringLiteral: String)

Creates an instance initialized to the given string value.

init(extendedGraphemeClusterLiteral: Self.StringLiteralType)

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for the `String` instance.

Deprecated

func withContiguousStorageIfAvailable&lt;R>((UnsafeBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R?

Executes a closure on the sequence’s contiguous storage.

