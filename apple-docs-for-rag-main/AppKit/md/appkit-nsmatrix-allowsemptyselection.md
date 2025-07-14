

- AppKit
- NSMatrix
-  allowsEmptySelection 

Instance Property

# allowsEmptySelection

A Boolean that indicates whether a radio-mode matrix supports an empty selection.

macOS

``` source
@MainActor
var allowsEmptySelection: Bool { get set }
```

## Discussion

When the value of this property is true, the matrix allows one or zero cells to be selected. When the value of this property is true, the matrix allows one and only one cell (not zero cells) to be selected. This setting has effect only in the `NSRadioModeMatrix` selection mode.

## See Also

### Configuring the Matrix Object

var mode: NSMatrix.Mode

The selection mode of the receiver.

var isSelectionByRect: Bool

A Boolean that indicates whether the user can select a rectangle of cells in the receiver by dragging the cursor.

