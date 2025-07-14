

- UIKit
- NSMutableParagraphStyle
-  lineBreakStrategy 

Instance Property

# lineBreakStrategy

The strategies that the text system may use to break lines while laying out the paragraph.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy { get set }
```

## Discussion

Line-break strategies are collections of options the system uses to determine where to break lines in a paragraph. This is different from lineBreakMode, which controls how to lay out lines of text that don’t fit in a container. The system ignores this property if the paragraph style’s lineBreakMode property specifies a mode that doesn’t support multiple lines, such as NSLineBreakMode.byClipping.

The default value is NSLineBreakStrategyNone.

## See Also

### Setting line-break information

var lineBreakMode: NSLineBreakMode

The mode for breaking lines in the paragraph.

var hyphenationFactor: Float

The paragraph’s threshold for hyphenation.

var usesDefaultHyphenation: Bool

var tighteningFactorForTruncation: Float { get set }

The threshold for using tightening as an alternative to truncation.

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that indicates whether the system tightens intercharacter spacing before truncating text.

