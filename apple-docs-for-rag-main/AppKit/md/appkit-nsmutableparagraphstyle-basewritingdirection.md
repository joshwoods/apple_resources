

- AppKit
- NSMutableParagraphStyle
-  baseWritingDirection 

Instance Property

# baseWritingDirection

The base writing direction for the paragraph.

macOS 10.0+

``` source
var baseWritingDirection: NSWritingDirection { get set }
```

## Discussion

If you specify NSWritingDirection.natural, the receiver resolves the writing direction to either NSWritingDirection.leftToRight or NSWritingDirection.rightToLeft, depending on the direction for the user’s language preference setting.

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

var paragraphSpacing: CGFloat

The space after the end of the paragraph.

var paragraphSpacingBefore: CGFloat

The distance between the paragraph’s top and the beginning of its text content.

