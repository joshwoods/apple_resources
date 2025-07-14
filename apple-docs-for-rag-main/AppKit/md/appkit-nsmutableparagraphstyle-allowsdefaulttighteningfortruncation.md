

- AppKit
- NSMutableParagraphStyle
-  allowsDefaultTighteningForTruncation 

Instance Property

# allowsDefaultTighteningForTruncation

A Boolean value that indicates whether the system tightens intercharacter spacing before truncating text.

macOS 10.11+

``` source
var allowsDefaultTighteningForTruncation: Bool { get set }
```

## Discussion

When this property is set to true, the system tries to reduce the space between characters before truncating characters. The system performs this tightening in cases where the text would not otherwise fit in the available space. The maximum amount of tightening performed by the system is dependent on the font, line width, and other factors.

The default value of this property is false.

## See Also

### Setting line-break information

var lineBreakMode: NSLineBreakMode

The mode for breaking lines in the paragraph.

var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy

The strategies that the text system may use to break lines while laying out the paragraph.

var hyphenationFactor: Float

The paragraph’s threshold for hyphenation.

var usesDefaultHyphenation: Bool

var tighteningFactorForTruncation: Float

The threshold for using tightening as an alternative to truncation.

