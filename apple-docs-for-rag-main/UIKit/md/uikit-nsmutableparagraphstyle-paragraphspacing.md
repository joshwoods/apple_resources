

- UIKit
- NSMutableParagraphStyle
-  paragraphSpacing 

Instance Property

# paragraphSpacing

The space after the end of the paragraph.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var paragraphSpacing: CGFloat { get set }
```

## Discussion

This property contains the space (measured in points) added at the end of the paragraph to separate it from the following paragraph. This value must be nonnegative. The space between paragraphs is determined by adding the previous paragraph’s `paragraphSpacing` and the current paragraph’s paragraphSpacingBefore.

## See Also

### Setting style information

func setParagraphStyle(NSParagraphStyle)

Replaces the subattributes of the paragraph with those in the specified paragraph style object.

var alignment: NSTextAlignment

The text alignment of the paragraph.

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

var paragraphSpacingBefore: CGFloat

The distance between the paragraph’s top and the beginning of its text content.

var baseWritingDirection: NSWritingDirection

The base writing direction for the paragraph.

