

- AppKit
- NSParagraphStyle
-  hyphenationFactor 

Instance Property

# hyphenationFactor

The paragraph’s threshold for hyphenation.

macOS 10.0+

``` source
var hyphenationFactor: Float { get }
```

## Discussion

The system attempts hyphenation when the ratio of the text width (as broken without hyphenation) to the width of the line fragment is less than the hyphenation factor. When the paragraph’s hyphenation factor is `0.0`, the system uses the layout manager’s hyphenation factor instead. The system disables hyphenation when both are `0.0`. This property detects the user-selected language by examining the first item in preferredLanguages.

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

var usesDefaultHyphenation: Bool

A Boolean value that indicates whether the paragraph style uses the system hyphenation settings.

var tighteningFactorForTruncation: Float

The threshold for using tightening as an alternative to truncation.

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that indicates whether the system tightens character spacing before truncating text.

