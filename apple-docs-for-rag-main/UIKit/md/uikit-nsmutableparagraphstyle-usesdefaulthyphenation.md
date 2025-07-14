

- UIKit
- NSMutableParagraphStyle
-  usesDefaultHyphenation 

Instance Property

# usesDefaultHyphenation

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var usesDefaultHyphenation: Bool { get set }
```

## See Also

### Setting line-break information

var lineBreakMode: NSLineBreakMode

The mode for breaking lines in the paragraph.

var lineBreakStrategy: NSParagraphStyle.LineBreakStrategy

The strategies that the text system may use to break lines while laying out the paragraph.

var hyphenationFactor: Float

The paragraph’s threshold for hyphenation.

var tighteningFactorForTruncation: Float { get set }

The threshold for using tightening as an alternative to truncation.

var allowsDefaultTighteningForTruncation: Bool

A Boolean value that indicates whether the system tightens intercharacter spacing before truncating text.

