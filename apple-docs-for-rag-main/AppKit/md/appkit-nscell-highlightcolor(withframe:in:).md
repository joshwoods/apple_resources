

- AppKit
- NSCell
-  highlightColor(withFrame:in:) 

Instance Method

# highlightColor(withFrame:in:)

Returns the color the receiver uses when drawing the selection highlight.

macOS

``` source
@MainActor
func highlightColor(
    withFrame cellFrame: NSRect,
    in controlView: NSView
) -> NSColor?
```

## Parameters 

`cellFrame`  

The bounding rectangle of the receiver.

`controlView`  

The control that manages the cell.

## Return Value

The color the receiver uses when drawing the selection highlight.

## Discussion

You should not assume that a cell would necessarily want to draw itself with the value returned from selectedControlColor. A cell may wish to draw with different a selection highlight color depending on such things as the key state of its `controlView`.

## See Also

### Drawing and Highlighting

func draw(withFrame: NSRect, in: NSView)

Draws the receiver’s border and then draws the interior of the cell.

func drawInterior(withFrame: NSRect, in: NSView)

Draws the interior portion of the receiver, which includes the image or text portion but does not include the border.

var controlView: NSView?

The view associated with the cell.

func highlight(Bool, withFrame: NSRect, in: NSView)

Redraws the receiver with the specified highlight setting.

var isHighlighted: Bool

A Boolean value indicating whether the cell has a highlighted appearance.

