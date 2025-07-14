

- AppKit
- NSParagraphStyle
-  minimumLineHeight 

Instance Property

# minimumLineHeight

The paragraph’s minimum line height.

macOS 10.0+

``` source
var minimumLineHeight: CGFloat { get }
```

## Discussion

This property contains the minimum height in points that any line in the receiver occupies, regardless of the font size or size of any attached graphic. This value is always nonnegative.

## See Also

### Accessing style information

var alignment: NSTextAlignment

The text alignment of the paragraph.

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

var lineSpacing: CGFloat

The distance in points between the bottom of one line fragment and the top of the next.

var paragraphSpacing: CGFloat

Distance between the bottom of this paragraph and top of next.

var paragraphSpacingBefore: CGFloat

The distance between the paragraph’s top and the beginning of its text content.

