

- AppKit
- NSParagraphStyle
-  tighteningFactorForTruncation 

Instance Property

# tighteningFactorForTruncation

The threshold for using tightening as an alternative to truncation.

macOS 10.0+

``` source
var tighteningFactorForTruncation: Float { get }
```

## Discussion

When the line break mode specifies truncation, the text system attempts to tighten character spacing as an alternative to truncation. Provided that the ratio of the text width to the line fragment width doesn’t exceed `1.0` + the system sets the tightening factor to this property. Otherwise, the system truncates the text at a location determined by the line break mode.

## See Also

### Getting line-break information

var lineBreakMode: NSLineBreakMode

The mode for breaking lines in the paragraph that don’t fit within a container.

enum NSLineBreakMode

Constants that specify what happens when a line is too long for a container.

var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy

The strategy for breaking lines while laying out paragraphs.

struct LineBreakStrategy

Constants that specify how the text system breaks lines while laying out paragraphs.

var hyphenationFactor: Float

The paragraph’s threshold for hyphenation.

var usesDefaultHyphenation: Bool

A Boolean value that indicates whether the paragraph style uses the system hyphenation settings.

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that indicates whether the system tightens character spacing before truncating text.

