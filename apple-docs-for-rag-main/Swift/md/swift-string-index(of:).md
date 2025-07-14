

- Swift
- String
-  index(of:) 

Instance Method

# index(of:)

Returns the first index where the specified value appears in the collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+SwiftDeprecated

``` source
func index(of element: Self.Element) -> Self.Index?
```

Available when `Element` conforms to `Equatable`.

## See Also

### Infrequently Used Functionality

init(NSString)

init(stringInterpolation: DefaultStringInterpolation)

Creates a new instance from an interpolated string literal.

init(stringLiteral: String)

Creates an instance initialized to the given string value.

init(unicodeScalarLiteral: Self.ExtendedGraphemeClusterLiteralType)

init(extendedGraphemeClusterLiteral: Self.StringLiteralType)

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for the `String` instance.

Deprecated

func withContiguousStorageIfAvailable&lt;R>((UnsafeBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R?

Executes a closure on the sequence’s contiguous storage.

