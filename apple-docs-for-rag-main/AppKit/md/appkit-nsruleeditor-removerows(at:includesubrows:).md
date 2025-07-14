

- AppKit
- NSRuleEditor
-  removeRows(at:includeSubrows:) 

Instance Method

# removeRows(at:includeSubrows:)

Removes the rows at given indexes.

macOS

``` source
@MainActor
func removeRows(
    at rowIndexes: IndexSet,
    includeSubrows: Bool
)
```

## Parameters 

`rowIndexes`  

Indexes of one or more rows in the receiver.

Important

Raises an `NSRangeException` if any index in `rowIndexes` is less than `0` or greater than or equal to the number of rows.

`includeSubrows`  

If true, then sub-rows of deleted rows are also deleted; if false, then each sub-row is adopted by its first non-deleted ancestor, or becomes a root row.

## See Also

### Manipulating Rows

func addRow(Any?)

Adds a row to the receiver.

func insertRow(at: Int, with: NSRuleEditor.RowType, asSubrowOfRow: Int, animate: Bool)

Adds a new row of a given type at a given location.

func removeRow(at: Int)

Removes the row at a given index.

