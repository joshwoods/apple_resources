

- AppKit
- NSParagraphStyle
-  lineHeightMultiple 

Instance Property

# lineHeightMultiple

The line height multiple.

macOS 10.0+

``` source
var lineHeightMultiple: CGFloat { get }
```

## Discussion

The framework multiplies the natural line height of the receiver by this factor (if positive), and constrains the resulting value by the minimum and maximum line height. The default value of this property is `0.0`.

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

