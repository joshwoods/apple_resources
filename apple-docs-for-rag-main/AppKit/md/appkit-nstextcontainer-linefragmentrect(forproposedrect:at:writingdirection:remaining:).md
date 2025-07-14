

- AppKit
- NSTextContainer
-  lineFragmentRect(forProposedRect:at:writingDirection:remaining:) 

Instance Method

# lineFragmentRect(forProposedRect:at:writingDirection:remaining:)

Returns the bounds of a line fragment rectangle inside the text container for the proposed rectangle.

macOS 10.11+

``` source
func lineFragmentRect(
    forProposedRect proposedRect: CGRect,
    at characterIndex: Int,
    writingDirection baseWritingDirection: NSWritingDirection,
    remaining remainingRect: UnsafeMutablePointer?
) -> CGRect
```

## Parameters 

`proposedRect`  

A rectangle in which to lay out text proposed by the layout manager.

`characterIndex`  

The character location inside the text storage for the line fragment being processed.

`baseWritingDirection`  

The direction of advancement for line fragments inside a visual horizontal line. The values passed into the method are either NSWritingDirection.leftToRight or NSWritingDirection.rightToLeft.

`remainingRect`  

The remainder of the proposed rectangle that was excluded from returned rectangle. It can be passed in as the proposed rectangle for the next iteration.

## Discussion

The bounds of the line fragment rectangle are determined by the intersection of `proposedRect` and the text container’s bounding rectangle defined by its NSTextContainer property. The regions defined by the NSTextContainer property are excluded from the return value. It is possible that `proposedRect` can be divided into multiple line fragments due to exclusion paths. In that case, `remainingRect` returns the remainder that can be passed in as the proposed rectangle for the next iteration.

This method can be overridden by subclasses for further text container region customization.

## See Also

### Constraining text layout

var maximumNumberOfLines: Int

The maximum number of lines that the text container can store.

var lineFragmentPadding: CGFloat

The value for the text inset within line fragment rectangles.

var isSimpleRectangularTextContainer: Bool

A Boolean that indicates whether the text container’s region is a rectangle with no holes or gaps, and whose edges are parallel to the text view’s coordinate system axes.

