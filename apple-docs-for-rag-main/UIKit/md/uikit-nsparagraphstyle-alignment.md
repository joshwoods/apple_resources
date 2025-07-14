

- UIKit
- NSParagraphStyle
-  alignment 

Instance Property

# alignment

The text alignment of the paragraph.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var alignment: NSTextAlignment { get }
```

## Discussion

The framework displays natural text alignment as left or right alignment depending on the line sweep direction of the first script contained in the paragraph.

## See Also

### Accessing style information

enum NSTextAlignment

Constants that specify text alignment.

var firstLineHeadIndent: CGFloat

The indentation of the first line of the paragraph.

var headIndent: CGFloat

The indentation of the paragraph’s lines other than the first.

var tailIndent: CGFloat

The trailing indentation of the paragraph.

var lineHeightMultiple: CGFloat

The line height multiple.

var maximumLineHeight: CGFloat

The paragraph’s maximum line height.

var minimumLineHeight: CGFloat

The paragraph’s minimum line height.

var lineSpacing: CGFloat

The distance in points between the bottom of one line fragment and the top of the next.

var paragraphSpacing: CGFloat

Distance between the bottom of this paragraph and top of next.

var paragraphSpacingBefore: CGFloat

The distance between the paragraph’s top and the beginning of its text content.

