

- Swift
- Unicode
- Unicode.Scalar
-  Unicode.Scalar.UTF16View 

Structure

# Unicode.Scalar.UTF16View

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct UTF16View
```

## Topics

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

RandomAccessCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- BitwiseCopyable
- Collection
- Copyable
- RandomAccessCollection
- Sendable
- Sequence

## See Also

### Printing and Displaying a Scalar

var description: String

A textual representation of the Unicode scalar.

func write&lt;Target>(to: inout Target)

Writes the textual representation of the Unicode scalar into the given output stream.

func escaped(asASCII: Bool) -> String

Returns a string representation of the Unicode scalar.

var utf16: Unicode.Scalar.UTF16View

var debugDescription: String

An escaped textual representation of the Unicode scalar, suitable for debugging.

var customMirror: Mirror

A mirror that reflects the `Unicode.Scalar` instance.

var customPlaygroundQuickLook: _PlaygroundQuickLook

A custom playground Quick Look for the `Unicode.Scalar` instance.

Deprecated

