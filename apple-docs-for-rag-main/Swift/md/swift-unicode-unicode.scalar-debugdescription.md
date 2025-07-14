

- Swift
- Unicode
- Unicode.Scalar
-  debugDescription 

Instance Property

# debugDescription

An escaped textual representation of the Unicode scalar, suitable for debugging.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var debugDescription: String { get }
```

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

var customMirror: Mirror

A mirror that reflects the `Unicode.Scalar` instance.

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for the `Unicode.Scalar` instance.

Deprecated

