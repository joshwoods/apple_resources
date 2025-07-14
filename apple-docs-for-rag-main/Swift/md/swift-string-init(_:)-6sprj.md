

- Swift
- String
-  init(\_:) 

Initializer

# init(\_:)

Creates a string corresponding to the given sequence of UTF-8 code units.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+Swift 4.0+

``` source
init(_ utf8: String.UTF8View)
```

## See Also

### Working with String Views

var unicodeScalars: String.UnicodeScalarView

The string’s value represented as a collection of Unicode scalar values.

init(String.UnicodeScalarView)

Creates a string corresponding to the given collection of Unicode scalars.

init(Substring.UnicodeScalarView)

Creates a String having the given content.

var utf16: String.UTF16View

A UTF-16 encoding of `self`.

init(String.UTF16View)

Creates a string corresponding to the given sequence of UTF-16 code units.

init?(Substring.UTF16View)

Creates a String having the given content.

var utf8: String.UTF8View

A UTF-8 encoding of `self`.

init?(Substring.UTF8View)

Creates a String having the given content.

