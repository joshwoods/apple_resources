

- AppKit
- NSTextContainer
-  contains(\_:) Deprecated

Instance Method

# contains(\_:)

Queries whether a point lies within the text container’s region or on the region’s edge—not simply within its bounding rectangle.

macOS 10.0–10.11Deprecated

``` source
func contains(_ point: NSPoint) -> Bool
```

## Parameters 

`point`  

The point in question.

## Return Value

true if `aPoint` lies within the receiver’s region or on the region’s edge—not simply within its bounding rectangle—false otherwise.

## Discussion

For example, if the receiver defines a donut shape and `aPoint` lies in the hole, this method returns false. This method can be used for hit testing of mouse events.

The default NSTextContainer implementation merely checks that `aPoint` lies within its bounding rectangle.

## See Also

### Deprecated

convenience init(containerSize: NSSize)

Initializes a text container with a specified bounding rectangle.

Deprecated

func lineFragmentRect(forProposedRect: NSRect, sweepDirection: NSLineSweepDirection, movementDirection: NSLineMovementDirection, remaining: NSRectPointer?) -> NSRect

Calculates and returns the longest rectangle available in the proposed rectangle for displaying text.

Deprecated

var containerSize: NSSize

The size of the text container’s bounding rectangle.

Deprecated

