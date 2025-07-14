

- AppKit
- NSTableColumn
-  isEditable 

Instance Property

# isEditable

A Boolean that indicates whether a cell-based table’s column cells are user editable.

macOS

``` source
@MainActor
var isEditable: Bool { get set }
```

## Discussion

When the value of this property is true, the user can edit cells in the cell-based table’s column. The default value of this property is true.

To initiate editing programmatically regardless of the value of this property, use the `NSTableView` editColumn(_:row:with:select:) method.

