

- AppKit
- NSCell
-  draw(withFrame:in:) 

Instance Method

# draw(withFrame:in:)

Draws the receiver’s border and then draws the interior of the cell.

macOS

``` source
@MainActor
func draw(
    withFrame cellFrame: NSRect,
    in controlView: NSView
)
```

## Parameters 

`cellFrame`  

The bounding rectangle of the receiver.

`controlView`  

The control that manages the cell.

## Discussion

This method draws the cell in the currently focused view, which can be different from the `controlView` passed in. Taking advantage of this behavior is not recommended, however.

## See Also

### Drawing and Highlighting

func highlightColor(withFrame: NSRect, in: NSView) -> NSColor?

Returns the color the receiver uses when drawing the selection highlight.

func drawInterior(withFrame: NSRect, in: NSView)

Draws the interior portion of the receiver, which includes the image or text portion but does not include the border.

var controlView: NSView?

The view associated with the cell.

func highlight(Bool, withFrame: NSRect, in: NSView)

Redraws the receiver with the specified highlight setting.

var isHighlighted: Bool

A Boolean value indicating whether the cell has a highlighted appearance.

