

- AppKit
- NSMutableParagraphStyle
-  tailIndent 

Instance Property

# tailIndent

The trailing indentation of the paragraph.

macOS 10.0+

``` source
var tailIndent: CGFloat { get set }
```

## Discussion

If positive, this value is the distance from the leading margin (for example, the left margin in left-to-right text). If 0 or negative, it’s the distance from the trailing margin.

For example, a paragraph style designed to fit exactly in a 2-inch wide container has a head indent of 0.0 and a tail indent of 0.0. One designed to fit with a quarter-inch margin has a head indent of 0.25 and a tail indent of –0.25.

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

