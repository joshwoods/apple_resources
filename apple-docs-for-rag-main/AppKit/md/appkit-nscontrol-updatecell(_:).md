

- AppKit
- NSControl
-  updateCell(\_:) 

Instance Method

# updateCell(\_:)

Marks the specified cell as in need of redrawing.

macOS

``` source
@MainActor
func updateCell(_ cell: NSCell)
```

## Parameters 

`cell`  

The cell to redraw.

## Discussion

If the cell currently has the focus, this method updates the cell’s focus ring; otherwise, the entire cell is marked as needing redisplay. The cell is redrawn during the next update cycle.

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

func drawCellInside(NSCell)

Draws the inside of the receiver’s cell (the area within the bezel or border)

func updateCellInside(NSCell)

Marks the inside of the specified cell as in need of redrawing.

