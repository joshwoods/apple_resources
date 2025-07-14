

- AppKit
- NSParagraphStyle
-  usesDefaultHyphenation 

Instance Property

# usesDefaultHyphenation

A Boolean value that indicates whether the paragraph style uses the system hyphenation settings.

macOS 12.0+

``` source
var usesDefaultHyphenation: Bool { get }
```

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

var tighteningFactorForTruncation: Float

The threshold for using tightening as an alternative to truncation.

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that indicates whether the system tightens character spacing before truncating text.

