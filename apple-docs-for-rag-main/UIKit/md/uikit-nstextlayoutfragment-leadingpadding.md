

- UIKit
- NSTextLayoutFragment
-  leadingPadding 

Instance Property

# leadingPadding

The amount of margin space reserved during paragraph layout between the leading edge of the text layout fragment and the start of the lines in the paragraph.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
var leadingPadding: CGFloat { get }
```

## Discussion

This is with respect to according to the primary writing direction of the paragraph and the start of the lines in the paragraph.

## See Also

### Defining margins and padding

var bottomMargin: CGFloat

The amount of space reserved during paragraph layout between the bottom of the last line in the paragraph and the bottom of the text layout fragment.

var topMargin: CGFloat

The amount of space reserved during paragraph layout between the top of the text layout fragment and the top of the first line in the paragraph.

var trailingPadding: CGFloat

The amount of margin space reserved during paragraph layout between the end of the lines in the paragraph and the trailing edge of the text layout fragment.

