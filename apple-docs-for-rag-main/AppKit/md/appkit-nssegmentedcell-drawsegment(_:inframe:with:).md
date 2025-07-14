

- AppKit
- NSSegmentedCell
-  drawSegment(\_:inFrame:with:) 

Instance Method

# drawSegment(\_:inFrame:with:)

Draws the image and label of the segment in the specified view.

macOS

``` source
@MainActor
func drawSegment(
    _ segment: Int,
    inFrame frame: NSRect,
    with controlView: NSView
)
```

## Parameters 

`segment`  

The index of the segment to draw. This method raises an exception (rangeException) if the index is out of bounds.

`frame`  

The rectangle in which to draw the segment’s image and label. This rectangle is specified in user space coordinates of the specified view.

`controlView`  

The view that contains the segment.

## Discussion

You can override this method to provide a custom appearance for segmented controls. You should not call this method directly. It is called for you automatically by the control when it needs to be redrawn.

## See Also

### Related Documentation

func draw(withFrame: NSRect, in: NSView)

Draws the receiver’s border and then draws the interior of the cell.

