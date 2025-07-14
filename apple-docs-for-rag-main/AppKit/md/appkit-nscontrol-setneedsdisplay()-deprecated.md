

- AppKit
- NSControl
-  setNeedsDisplay() Deprecated

Instance Method

# setNeedsDisplay()

Marks the receiver as needing redisplay (assuming automatic display is enabled).

macOS 10.0–10.14Deprecated

``` source
@MainActor
func setNeedsDisplay()
```

Deprecated

Set the needsDisplay property to YES instead

## Discussion

This method also recalculates the dimensions of the control as needed.

## See Also

### Related Documentation

var needsDisplay: Bool

A Boolean value that determines whether the view needs to be redrawn before being displayed.

### Deprecated Methods

func selectedCell() -> NSCell?

Returns the receiver’s selected cell.

func selectedTag() -> Int

Returns the tag of the receiver’s selected cell.

func calcSize()

Recomputes any internal sizing information for the receiver, if necessary.

Deprecated

func selectCell(NSCell)

Selects the specified cell and redraws the control as needed.

func drawCell(NSCell)

Draws the specified cell, as long as it belongs to the receiver.

func drawCellInside(NSCell)

Draws the inside of the receiver’s cell (the area within the bezel or border)

func updateCell(NSCell)

Marks the specified cell as in need of redrawing.

func updateCellInside(NSCell)

Marks the inside of the specified cell as in need of redrawing.

