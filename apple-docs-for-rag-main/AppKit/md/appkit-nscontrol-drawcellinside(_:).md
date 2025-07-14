

- AppKit
- NSControl
-  drawCellInside(\_:) 

Instance Method

# drawCellInside(\_:)

Draws the inside of the receiver’s cell (the area within the bezel or border)

macOS

``` source
@MainActor
func drawCellInside(_ cell: NSCell)
```

## Parameters 

`cell`  

The cell to draw. If the cell does not belong to the receiver, this method does nothing.

## Discussion

If the receiver is transparent, the method causes the superview to draw itself. This method invokes the drawInterior(withFrame:in:) method of NSCell. This method has no effect on controls (such as `NSMatrix` and `NSForm`) that have multiple cells.

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

func drawCell(NSCell)

Draws the specified cell, as long as it belongs to the receiver.

func updateCell(NSCell)

Marks the specified cell as in need of redrawing.

func updateCellInside(NSCell)

Marks the inside of the specified cell as in need of redrawing.

