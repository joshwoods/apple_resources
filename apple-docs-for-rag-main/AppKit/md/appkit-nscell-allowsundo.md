

- AppKit
- NSCell
-  allowsUndo 

Instance Property

# allowsUndo

A Boolean value indicating whether the cell assumes responsibility for undo operations.

macOS

``` source
@MainActor
var allowsUndo: Bool { get set }
```

## Discussion

The value of this property is true if the cell handles undo operations itself or false if the app’s custom undo manager must handle undo behavior. Cell subclasses set the value of this property to indicate their preference for handling undo operations. For example, the NSTextFieldCell class uses sets this property to indicate it handles undo operations for edited text, and other controls set a value that is appropriate for their implementation. Do not change the value of this property otherwise.

## See Also

### Managing Cell Attributes

func setCellAttribute(NSCell.Attribute, to: Int)

Sets the value for the specified cell attribute.

func cellAttribute(NSCell.Attribute) -> Int

Returns the value for the specified cell attribute.

var type: NSCell.CellType

The type of the cell.

var isEnabled: Bool

A Boolean value indicating whether the cell is currently enabled.

