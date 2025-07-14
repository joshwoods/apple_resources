

- AppKit
- NSControl
-  selectCell(\_:) 

Instance Method

# selectCell(\_:)

Selects the specified cell and redraws the control as needed.

macOS

``` source
@MainActor
func selectCell(_ cell: NSCell)
```

## Parameters 

`cell`  

The cell to select. The cell must belong to the receiver.

## Discussion

If the cell is already selected (or does not belong to the receiver), this method does nothing. If the cell belongs to the receiver and is not selected, this method changes its state to `NSOnState` and redraws the cell.

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

func drawCell(NSCell)

Draws the specified cell, as long as it belongs to the receiver.

func drawCellInside(NSCell)

Draws the inside of the receiver’s cell (the area within the bezel or border)

func updateCell(NSCell)

Marks the specified cell as in need of redrawing.

func updateCellInside(NSCell)

Marks the inside of the specified cell as in need of redrawing.

