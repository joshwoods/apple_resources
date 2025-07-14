

- UIKit
- NSParagraphStyle
-  lineBreakMode 

Instance Property

# lineBreakMode

The mode for breaking lines in the paragraph that don’t fit within a container.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var lineBreakMode: NSLineBreakMode { get }
```

## Discussion

This property controls how the text system lays out lines that don’t fit in its container, such as by truncating with an ellipsis (…) or clipping the text. This is different from NSParagraphStyle.LineBreakStrategy, which controls where the system places line breaks in a paragraph.

## See Also

### Getting line-break information

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

var tighteningFactorForTruncation: Float { get }

The threshold for using tightening as an alternative to truncation.

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that indicates whether the system tightens character spacing before truncating text.

