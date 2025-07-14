

- Swift
- AsyncSequence
-  characters 

Instance Property

# characters

A non-blocking sequence of `Characters` created by decoding the elements of `self` as UTF8.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var characters: AsyncCharacterSequence { get }
```

Available when `Element` is `UInt8`.

## See Also

### Adapting Textual Sequences

struct AsyncCharacterSequence

An asychronous sequence of characters.

var unicodeScalars: AsyncUnicodeScalarSequence&lt;Self>

A non-blocking sequence of `UnicodeScalars` created by decoding the elements of `self` as UTF8.

struct AsyncUnicodeScalarSequence

An asychronous sequence of Unicode scalar values.

var lines: AsyncLineSequence&lt;Self>

A non-blocking sequence of newline-separated `Strings` created by decoding the elements of `self` as UTF8.

struct AsyncLineSequence

An asychronous sequence of lines of text.

