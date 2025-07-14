

- AppKit
- NSMutableParagraphStyle
-  alignment 

Instance Property

# alignment

The text alignment of the paragraph.

macOS 10.0+

``` source
var alignment: NSTextAlignment { get set }
```

## Discussion

Natural text alignment is realized as left or right alignment depending on the line sweep direction of the first script contained in the paragraph.

## See Also

### Setting style information

func setParagraphStyle(NSParagraphStyle)

Replaces the subattributes of the paragraph with those in the specified paragraph style object.

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

The space after the end of the paragraph.

var paragraphSpacingBefore: CGFloat

The distance between the paragraph’s top and the beginning of its text content.

var baseWritingDirection: NSWritingDirection

The base writing direction for the paragraph.

