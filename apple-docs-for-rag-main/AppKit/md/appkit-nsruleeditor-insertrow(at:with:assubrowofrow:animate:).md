

- AppKit
- NSRuleEditor
-  insertRow(at:with:asSubrowOfRow:animate:) 

Instance Method

# insertRow(at:with:asSubrowOfRow:animate:)

Adds a new row of a given type at a given location.

macOS

``` source
@MainActor
func insertRow(
    at rowIndex: Int,
    with rowType: NSRuleEditor.RowType,
    asSubrowOfRow parentRow: Int,
    animate shouldAnimate: Bool
)
```

## Parameters 

`rowIndex`  

The index at which the new row should be inserted. `rowIndex` must be greater than `parentRow`, and much specify a row that does not fall amongst the children of some other parent.

`rowType`  

The type of the new row.

`parentRow`  

The index of the row of which the new row is a child. Pass `-1` to indicate that the new row should be a root row.

`shouldAnimate`  

true if creation of the new row should be animated, otherwise false.

## Discussion

Important

If `parentRow` is greater than or equal to `rowIndex`, or if `rowIndex` would fall amongst the children of some other parent, or if the nesting mode forbids this configuration, an `NSInvalidArgumentException` is raised.

## See Also

### Manipulating Rows

func addRow(Any?)

Adds a row to the receiver.

func removeRow(at: Int)

Removes the row at a given index.

func removeRows(at: IndexSet, includeSubrows: Bool)

Removes the rows at given indexes.

