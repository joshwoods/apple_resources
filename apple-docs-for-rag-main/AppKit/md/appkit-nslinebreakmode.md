

- AppKit
-  NSLineBreakMode 

Enumeration

# NSLineBreakMode

Constants that specify what happens when a line is too long for a container.

macOS 10.0+

``` source
enum NSLineBreakMode
```

## Topics

### Constants

case byWordWrapping

The value that indicates wrapping occurs at word boundaries, unless the word doesn’t fit on a single line.

case byCharWrapping

The value that indicates wrapping occurs before the first character that doesn’t fit.

case byClipping

The value that indicates lines don’t extend past the edge of the text container.

case byTruncatingHead

The value that indicates that a line displays so that the end fits in the container and an ellipsis glyph indicates the missing text at the beginning of the line.

case byTruncatingTail

The value that indicates a line displays so that the beginning fits in the container and an ellipsis glyph indicates the missing text at the end of the line.

case byTruncatingMiddle

The value that indicates that a line displays so that the beginning and end fit in the container and an ellipsis glyph indicates the missing text in the middle.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting line-break information

var lineBreakMode: NSLineBreakMode

The mode for breaking lines in the paragraph that don’t fit within a container.

var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy

The strategy for breaking lines while laying out paragraphs.

struct LineBreakStrategy

Constants that specify how the text system breaks lines while laying out paragraphs.

var hyphenationFactor: Float

The paragraph’s threshold for hyphenation.

var usesDefaultHyphenation: Bool

A Boolean value that indicates whether the paragraph style uses the system hyphenation settings.

var tighteningFactorForTruncation: Float

The threshold for using tightening as an alternative to truncation.

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that indicates whether the system tightens character spacing before truncating text.

