

- Swift
- Unicode
- Unicode.Scalar
-  customPlaygroundQuickLook Deprecated

Instance Property

# customPlaygroundQuickLook

A custom playground Quick Look for the `Unicode.Scalar` instance.

iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+iOS 8.0+

``` source
var customPlaygroundQuickLook: _PlaygroundQuickLook { get }
```

Deprecated

Unicode.Scalar.customPlaygroundQuickLook will be removed in a future Swift version

## See Also

### Printing and Displaying a Scalar

var description: String

A textual representation of the Unicode scalar.

func write&lt;Target>(to: inout Target)

Writes the textual representation of the Unicode scalar into the given output stream.

func escaped(asASCII: Bool) -> String

Returns a string representation of the Unicode scalar.

var utf16: Unicode.Scalar.UTF16View

struct UTF16View

var debugDescription: String

An escaped textual representation of the Unicode scalar, suitable for debugging.

var customMirror: Mirror

A mirror that reflects the `Unicode.Scalar` instance.

