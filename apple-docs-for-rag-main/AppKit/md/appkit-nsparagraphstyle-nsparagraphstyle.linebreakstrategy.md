

- AppKit
- NSParagraphStyle
-  NSParagraphStyle.LineBreakStrategy 

Structure

# NSParagraphStyle.LineBreakStrategy

Constants that specify how the text system breaks lines while laying out paragraphs.

macOS 10.11+

``` source
struct LineBreakStrategy
```

## Topics

### Getting the line-break styles

static var pushOut: NSParagraphStyle.LineBreakStrategy

The text system pushes out individual lines to avoid an orphan word on the last line of the paragraph.

static var hangulWordPriority: NSParagraphStyle.LineBreakStrategy

The text system prohibits breaking between Hangul characters.

static var standard: NSParagraphStyle.LineBreakStrategy

The text system uses the same configuration of line-break strategies that it uses for standard UI labels.

### Creating a line-break style

init(rawValue: UInt)

Creates a line-break strategy with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Getting line-break information

var lineBreakMode: NSLineBreakMode

The mode for breaking lines in the paragraph that don’t fit within a container.

enum NSLineBreakMode

Constants that specify what happens when a line is too long for a container.

var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy

The strategy for breaking lines while laying out paragraphs.

var hyphenationFactor: Float

The paragraph’s threshold for hyphenation.

var usesDefaultHyphenation: Bool

A Boolean value that indicates whether the paragraph style uses the system hyphenation settings.

var tighteningFactorForTruncation: Float

The threshold for using tightening as an alternative to truncation.

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that indicates whether the system tightens character spacing before truncating text.

