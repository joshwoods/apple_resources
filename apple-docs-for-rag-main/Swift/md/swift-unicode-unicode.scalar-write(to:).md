

- Swift
- Unicode
- Unicode.Scalar
-  write(to:) 

Instance Method

# write(to:)

Writes the textual representation of the Unicode scalar into the given output stream.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func write(to target: inout Target) where Target : TextOutputStream
```

## Parameters 

`target`  

An output stream.

## See Also

### Printing and Displaying a Scalar

var description: String

A textual representation of the Unicode scalar.

func escaped(asASCII: Bool) -> String

Returns a string representation of the Unicode scalar.

var utf16: Unicode.Scalar.UTF16View

struct UTF16View

var debugDescription: String

An escaped textual representation of the Unicode scalar, suitable for debugging.

var customMirror: Mirror

A mirror that reflects the `Unicode.Scalar` instance.

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for the `Unicode.Scalar` instance.

Deprecated

