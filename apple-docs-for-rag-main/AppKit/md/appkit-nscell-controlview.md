

- AppKit
- NSCell
-  controlView 

Instance Property

# controlView

The view associated with the cell.

macOS

``` source
@MainActor
unowned(unsafe) var controlView: NSView? { get set }
```

## Discussion

This property contains the view associated with the cell. This view is normally an NSControl object. The default value of this property is `nil`.

## See Also

### Drawing and Highlighting

func draw(withFrame: NSRect, in: NSView)

Draws the receiver’s border and then draws the interior of the cell.

func highlightColor(withFrame: NSRect, in: NSView) -> NSColor?

Returns the color the receiver uses when drawing the selection highlight.

func drawInterior(withFrame: NSRect, in: NSView)

Draws the interior portion of the receiver, which includes the image or text portion but does not include the border.

func highlight(Bool, withFrame: NSRect, in: NSView)

Redraws the receiver with the specified highlight setting.

var isHighlighted: Bool

A Boolean value indicating whether the cell has a highlighted appearance.

