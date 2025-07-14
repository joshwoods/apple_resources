

- AppKit
- NSMutableParagraphStyle
-  tighteningFactorForTruncation 

Instance Property

# tighteningFactorForTruncation

The threshold for using tightening as an alternative to truncation.

macOS 10.0+

``` source
var tighteningFactorForTruncation: Float { get set }
```

## Discussion

When the line break mode specifies truncation, the text system attempts to tighten inter character spacing as an alternative to truncation, provided that the ratio of the text width to the line fragment width does not exceed 1.0 + the value of tighteningFactorForTruncation. Otherwise the text is truncated at a location determined by the line break mode. The default value is 0.05. This value can be a positive or negative value. Values less than or equal to 0.0 result in not tightening.

## See Also

### Setting line-break information

var lineBreakMode: NSLineBreakMode

The mode for breaking lines in the paragraph.

var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy

The strategies that the text system may use to break lines while laying out the paragraph.

var hyphenationFactor: Float

The paragraph’s threshold for hyphenation.

var usesDefaultHyphenation: Bool

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that indicates whether the system tightens intercharacter spacing before truncating text.

