

- AppKit
- NSCell
-  highlight(\_:withFrame:in:) 

Instance Method

# highlight(\_:withFrame:in:)

Redraws the receiver with the specified highlight setting.

macOS

``` source
@MainActor
func highlight(
    _ flag: Bool,
    withFrame cellFrame: NSRect,
    in controlView: NSView
)
```

## Parameters 

`flag`  

If true, the cell is redrawn with a highlight; otherwise, if false, the highlight is removed.

`cellFrame`  

The bounding rectangle of the receiver.

`controlView`  

The control that manages the cell.

## Discussion

Note that the `NSCell` highlighting does not appear when highlighted cells are printed (although instances of `NSTextFieldCell`, `NSButtonCell`, and others can print themselves highlighted). Generally, you cannot depend on highlighting being printed because implementations of this method may choose (or not choose) to use transparency.

## See Also

### Drawing and Highlighting

func draw(withFrame: NSRect, in: NSView)

Draws the receiver’s border and then draws the interior of the cell.

func highlightColor(withFrame: NSRect, in: NSView) -> NSColor?

Returns the color the receiver uses when drawing the selection highlight.

func drawInterior(withFrame: NSRect, in: NSView)

Draws the interior portion of the receiver, which includes the image or text portion but does not include the border.

var controlView: NSView?

The view associated with the cell.

var isHighlighted: Bool

A Boolean value indicating whether the cell has a highlighted appearance.

