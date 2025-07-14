

- AppKit
- NSRuleEditor
-  removeRow(at:) 

Instance Method

# removeRow(at:)

Removes the row at a given index.

macOS

``` source
@MainActor
func removeRow(at rowIndex: Int)
```

## Parameters 

`rowIndex`  

The index of a row in the receiver.

Important

Raises an `NSRangeException` if `rowIndex` is less than `0` or greater than or equal to the number of rows.

## Discussion

Any subrows of the deleted row are adopted by the parent of the deleted row, or are made root rows.

## See Also

### Manipulating Rows

func addRow(Any?)

Adds a row to the receiver.

func insertRow(at: Int, with: NSRuleEditor.RowType, asSubrowOfRow: Int, animate: Bool)

Adds a new row of a given type at a given location.

func removeRows(at: IndexSet, includeSubrows: Bool)

Removes the rows at given indexes.

