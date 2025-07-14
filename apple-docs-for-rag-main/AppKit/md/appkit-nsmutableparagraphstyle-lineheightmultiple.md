

- AppKit
- NSMutableParagraphStyle
-  lineHeightMultiple 

Instance Property

# lineHeightMultiple

The line height multiple.

macOS 10.0+

``` source
var lineHeightMultiple: CGFloat { get set }
```

## Discussion

The natural line height of the receiver is multiplied by this factor (if positive) before being constrained by minimum and maximum line height. The default value of this property is 0.0.

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

