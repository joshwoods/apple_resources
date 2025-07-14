

- AppKit
- NSParagraphStyle
-  headIndent 

Instance Property

# headIndent

The indentation of the paragraph’s lines other than the first.

macOS 10.0+

``` source
var headIndent: CGFloat { get }
```

## Discussion

This property contains the distance (in points) from the leading margin of a text container to the beginning of lines other than the first. This value is always nonnegative.

## See Also

### Accessing style information

var alignment: NSTextAlignment

The text alignment of the paragraph.

enum NSTextAlignment

Constants that specify text alignment.

var firstLineHeadIndent: CGFloat

The indentation of the first line of the paragraph.

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

