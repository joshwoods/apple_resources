

- AppKit
- NSCell
-  type 

Instance Property

# type

The type of the cell.

macOS

``` source
@MainActor
var type: NSCell.CellType { get set }
```

## Discussion

When you change the cell type to NSCell.CellType.textCellType, the cell converts gives itself a default title and sets the font to the system font at the default size. When you change the cell type to NSCell.CellType.imageCellType, the cell type does not change until you assign a new non-`nil` image to it.

For a list of possible cell types, see NSCell.CellType.

## See Also

### Related Documentation

var image: NSImage?

The image displayed by the cell, if any.

### Managing Cell Attributes

func setCellAttribute(NSCell.Attribute, to: Int)

Sets the value for the specified cell attribute.

func cellAttribute(NSCell.Attribute) -> Int

Returns the value for the specified cell attribute.

var isEnabled: Bool

A Boolean value indicating whether the cell is currently enabled.

var allowsUndo: Bool

A Boolean value indicating whether the cell assumes responsibility for undo operations.

