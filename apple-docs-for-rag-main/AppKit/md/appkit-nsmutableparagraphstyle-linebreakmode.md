

- AppKit
- NSMutableParagraphStyle
-  lineBreakMode 

Instance Property

# lineBreakMode

The mode for breaking lines in the paragraph.

macOS 10.0+

``` source
var lineBreakMode: NSLineBreakMode { get set }
```

## Discussion

This property controls how the text system lays out lines that don’t fit in its container, such as by truncating with an ellipsis (…) or clipping the text. This is different from NSParagraphStyle.LineBreakStrategy , which controls where the system places line breaks in a paragraph.

## See Also

### Setting line-break information

var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy

The strategies that the text system may use to break lines while laying out the paragraph.

var hyphenationFactor: Float

The paragraph’s threshold for hyphenation.

var usesDefaultHyphenation: Bool

var tighteningFactorForTruncation: Float

The threshold for using tightening as an alternative to truncation.

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that indicates whether the system tightens intercharacter spacing before truncating text.

