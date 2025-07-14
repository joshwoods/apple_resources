

- UIKit
- NSParagraphStyle
-  tailIndent 

Instance Property

# tailIndent

The trailing indentation of the paragraph.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var tailIndent: CGFloat { get }
```

## Discussion

If positive, this value is the distance from the leading margin (for example, the left margin in left-to-right text). If `0` or negative, it’s the distance from the trailing margin.

For example, a paragraph style designed to fit exactly in a two-inch wide container has a head indent of `0.0` and a tail indent of `0.0`. One designed to fit with a quarter-inch margin has a head indent of `0.25` and a tail indent of `–0.25`.

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

