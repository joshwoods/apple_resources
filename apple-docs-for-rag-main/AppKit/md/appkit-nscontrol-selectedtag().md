

- AppKit
- NSControl
-  selectedTag() 

Instance Method

# selectedTag()

Returns the tag of the receiver’s selected cell.

macOS

``` source
@MainActor
func selectedTag() -> Int
```

## Return Value

The tag of the selected cell, or `-1` if no cell is selected.

## Discussion

When you set the tag of a control with a single cell in Interface Builder, it sets the tags of both the control and the cell with the same value as a convenience.

## See Also

### Related Documentation

var tag: Int

The tag identifying the receiver (not the tag of the receiver’s cell).

### Deprecated Methods

func selectedCell() -> NSCell?

Returns the receiver’s selected cell.

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

