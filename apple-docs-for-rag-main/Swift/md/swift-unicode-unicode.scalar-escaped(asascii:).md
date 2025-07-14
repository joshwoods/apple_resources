

- Swift
- Unicode
- Unicode.Scalar
-  escaped(asASCII:) 

Instance Method

# escaped(asASCII:)

Returns a string representation of the Unicode scalar.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func escaped(asASCII forceASCII: Bool) -> String
```

## Parameters 

`forceASCII`  

Pass `true` if you need the result to use only ASCII characters; otherwise, pass `false`.

## Return Value

A string representation of the scalar.

## Discussion

Scalar values representing characters that are normally unprintable or that otherwise require escaping are escaped with a backslash.

```
let tab = Unicode.Scalar(9)!
print(tab)
// Prints " "
print(tab.escaped(asASCII: false))
// Prints "\t"
```

When the `forceASCII` parameter is `true`, a `Unicode.Scalar` instance with a value greater than 127 is represented using an escaped numeric value; otherwise, non-ASCII characters are represented using their typical string value.

```
let bap = Unicode.Scalar(48165)!
print(bap.escaped(asASCII: false))
// Prints "밥"
print(bap.escaped(asASCII: true))
// Prints "\u{BC25}"
```

## See Also

### Printing and Displaying a Scalar

var description: String

A textual representation of the Unicode scalar.

func write&lt;Target>(to: inout Target)

Writes the textual representation of the Unicode scalar into the given output stream.

var utf16: Unicode.Scalar.UTF16View

struct UTF16View

var debugDescription: String

An escaped textual representation of the Unicode scalar, suitable for debugging.

var customMirror: Mirror

A mirror that reflects the `Unicode.Scalar` instance.

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for the `Unicode.Scalar` instance.

Deprecated

