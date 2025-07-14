

- AppKit
- NSCell
-  isHighlighted 

Instance Property

# isHighlighted

A Boolean value indicating whether the cell has a highlighted appearance.

macOS

``` source
@MainActor
var isHighlighted: Bool { get set }
```

## Discussion

When the value of this property is true, the cell draws itself with a highlighted appearance. The default value of this property is false.

Assigning a new value to this property has no effect by default. Subclasses can override the property to provide a highlighting behavior. For example, the NSButtonCell class overrides this property, so that when the value is true the button draws the button with a highlight appearance specified by NSCell.Attribute.cellLightsByBackground, NSCell.Attribute.cellLightsByContents, or NSCell.Attribute.cellLightsByGray.

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

func highlight(Bool, withFrame: NSRect, in: NSView)

Redraws the receiver with the specified highlight setting.

