

- AppKit
- NSTextContainer
-  lineFragmentRect(forProposedRect:sweepDirection:movementDirection:remaining:) Deprecated

Instance Method

# lineFragmentRect(forProposedRect:sweepDirection:movementDirection:remaining:)

Calculates and returns the longest rectangle available in the proposed rectangle for displaying text.

macOS

``` source
func lineFragmentRect(
    forProposedRect proposedRect: NSRect,
    sweepDirection: NSLineSweepDirection,
    movementDirection: NSLineMovementDirection,
    remaining remainingRect: NSRectPointer?
) -> NSRect
```

Deprecated

Use lineFragmentRect(forProposedRect:at:writingDirection:remaining:) instead.

## Parameters 

`proposedRect`  

The proposed rectangle in which to layout text.

`sweepDirection`  

The line sweep direction.

`movementDirection`  

The line movement direction.

`remainingRect`  

Upon return, the unused, possibly shifted, portion of `proposedRect` that’s available for further text, or `NSZeroRect` if there is no remainder.

## Return Value

The longest rectangle available in the proposed rectangle for displaying text, or `NSZeroRect` if there is none according to the receiver’s region definition.

## Discussion

There is no guarantee as to the width of the proposed rectangle or to its location. For example, the proposed rectangle is likely to be much wider than the width of the receiver. The receiver should examine `proposedRect` to see that it intersects its bounding rectangle and should return a modified rectangle based on `sweepDirection` and `movementDirection`, whose possible values are listed in the class description. If `sweepDirection` is `NSLineSweepRight`, for example, the receiver uses this information to trim the right end of `proposedRect` as needed rather than the left end.

If `proposedRect` doesn’t completely overlap the region along the axis of `movementDirection` and `movementDirection` isn’t `NSLineDoesntMove`, this method can either shift the rectangle in that direction as much as needed so that it does completely overlap, or return `NSZeroRect` to indicate that the proposed rectangle simply doesn’t fit.

## See Also

### Deprecated

convenience init(containerSize: NSSize)

Initializes a text container with a specified bounding rectangle.

Deprecated

func contains(NSPoint) -> Bool

Queries whether a point lies within the text container’s region or on the region’s edge—not simply within its bounding rectangle.

Deprecated

var containerSize: NSSize

The size of the text container’s bounding rectangle.

Deprecated

