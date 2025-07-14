

- AppKit
- NSCell
-  cellAttribute(\_:) 

Instance Method

# cellAttribute(\_:)

Returns the value for the specified cell attribute.

macOS

``` source
@MainActor
func cellAttribute(_ parameter: NSCell.Attribute) -> Int
```

## Parameters 

`parameter`  

The cell attribute whose value you want to get. Attributes include the receiver’s current state and whether it is disabled, editable, or highlighted.

## Return Value

The value for the cell attribute specified by `aParameter`.

## See Also

### Managing Cell Attributes

func setCellAttribute(NSCell.Attribute, to: Int)

Sets the value for the specified cell attribute.

var type: NSCell.CellType

The type of the cell.

var isEnabled: Bool

A Boolean value indicating whether the cell is currently enabled.

var allowsUndo: Bool

A Boolean value indicating whether the cell assumes responsibility for undo operations.

