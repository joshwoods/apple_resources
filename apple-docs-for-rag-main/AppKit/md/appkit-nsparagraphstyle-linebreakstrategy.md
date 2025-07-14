

- AppKit
- NSParagraphStyle
-  lineBreakStrategy 

Instance Property

# lineBreakStrategy

The strategy for breaking lines while laying out paragraphs.

macOS 10.11+

``` source
var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy { get }
```

## Discussion

Line-break strategies are collections of options the system uses to determine where to break lines in a paragraph. This is different from lineBreakMode, which controls how to lay out lines of text that don’t fit in a container. The system ignores this property if the paragraph style’s lineBreakMode property specifies a mode that doesn’t support multiple lines, such as NSLineBreakMode.byClipping.

The default value is NSLineBreakStrategyNone.

## See Also

### Getting line-break information

var lineBreakMode: NSLineBreakMode

The mode for breaking lines in the paragraph that don’t fit within a container.

enum NSLineBreakMode

Constants that specify what happens when a line is too long for a container.

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

