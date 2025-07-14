

- AppKit
- NSControl
-  selectedCell() 

Instance Method

# selectedCell()

Returns the receiver’s selected cell.

macOS

``` source
@MainActor
func selectedCell() -> NSCell?
```

## Return Value

The selected cell object.

## Discussion

The default implementation of this method simply returns the control’s associated cell (or `nil` if no cell has been set). Subclasses of `NSControl` that manage multiple cells (such as `NSMatrix` and `NSForm`) must override this method to return the cell selected by the user.

## See Also

### Related Documentation

var cell: NSCell?

The receiver’s cell object.

### Deprecated Methods

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

func updateCell(NSCell)

Marks the specified cell as in need of redrawing.

func updateCellInside(NSCell)

Marks the inside of the specified cell as in need of redrawing.

