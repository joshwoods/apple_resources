

- AppKit
- NSCell
-  isEnabled 

Instance Property

# isEnabled

A Boolean value indicating whether the cell is currently enabled.

macOS

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

The value of this property is true when the cell is enabled or false when it is disabled. The text of disabled cells is gray. If a cell is disabled, it cannot be highlighted, does not support mouse tracking (and thus cannot participate in target/action functionality), and cannot be edited. However, you can still alter many attributes of a disabled cell programmatically. (The state property, for instance, still works.)

## See Also

### Managing Cell Attributes

func setCellAttribute(NSCell.Attribute, to: Int)

Sets the value for the specified cell attribute.

func cellAttribute(NSCell.Attribute) -> Int

Returns the value for the specified cell attribute.

var type: NSCell.CellType

The type of the cell.

var allowsUndo: Bool

A Boolean value indicating whether the cell assumes responsibility for undo operations.

