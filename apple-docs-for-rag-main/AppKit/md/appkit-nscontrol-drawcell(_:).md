

- AppKit
- NSControl
-  drawCell(\_:) 

Instance Method

# drawCell(\_:)

Draws the specified cell, as long as it belongs to the receiver.

macOS

``` source
@MainActor
func drawCell(_ cell: NSCell)
```

## Parameters 

`cell`  

The cell to draw. If the cell does not belong to the receiver, this method does nothing.

## Discussion

This method is provided primarily to support a consistent set of methods between `NSControl` objects with single and multiple cells, because a control with multiple cells needs to be able to draw individual cells.

## See Also

### Deprecated Methods

func selectedCell() -> NSCell?

Returns the receiver’s selected cell.

func selectedTag() -> Int

Returns the tag of the receiver’s selected cell.

func setNeedsDisplay()

Marks the receiver as needing redisplay (assuming automatic display is enabled).

Deprecated

func calcSize()

Recomputes any internal sizing information for the receiver, if necessary.

Deprecated

func selectCell(NSCell)

Selects the specified cell and redraws the control as needed.

func drawCellInside(NSCell)

Draws the inside of the receiver’s cell (the area within the bezel or border)

func updateCell(NSCell)

Marks the specified cell as in need of redrawing.

func updateCellInside(NSCell)

Marks the inside of the specified cell as in need of redrawing.

