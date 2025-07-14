

- AppKit
- NSMatrix
-  isSelectionByRect 

Instance Property

# isSelectionByRect

A Boolean that indicates whether the user can select a rectangle of cells in the receiver by dragging the cursor.

macOS

``` source
@MainActor
var isSelectionByRect: Bool { get set }
```

## Discussion

When the value of this property is true, the matrix allows the user to select a rectangle of cells by dragging. When the value of this property is false, selection in the matrix is on a row-by-row basis. The default value of this property is true.

## See Also

### Related Documentation

func setSelectionFrom(Int, to: Int, anchor: Int, highlight: Bool)

Programmatically selects a range of cells.

### Configuring the Matrix Object

var mode: NSMatrix.Mode

The selection mode of the receiver.

var allowsEmptySelection: Bool

A Boolean that indicates whether a radio-mode matrix supports an empty selection.

