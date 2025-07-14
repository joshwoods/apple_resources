

- AppKit
- NSControl
-  calcSize() Deprecated

Instance Method

# calcSize()

Recomputes any internal sizing information for the receiver, if necessary.

macOS 10.0–10.14Deprecated

``` source
@MainActor
func calcSize()
```

Deprecated

Override -layout instead. This method should never be called

## Discussion

This method uses the calcDrawInfo(_:) method of its cell to perform the calculations. Most controls maintain a flag that informs them if any of their cells have been modified in such a way that the location or size of the cell should be recomputed. If such a modification happens, this method is automatically invoked before the control is displayed. You should never need to invoke it yourself.

## See Also

### Related Documentation

func sizeToFit()

Resizes the receiver’s frame so that it’s the minimum size needed to contain its cell.

### Deprecated Methods

func selectedCell() -> NSCell?

Returns the receiver’s selected cell.

func selectedTag() -> Int

Returns the tag of the receiver’s selected cell.

func setNeedsDisplay()

Marks the receiver as needing redisplay (assuming automatic display is enabled).

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

