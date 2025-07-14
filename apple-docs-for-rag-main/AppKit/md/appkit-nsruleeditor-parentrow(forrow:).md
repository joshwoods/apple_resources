

- AppKit
- NSRuleEditor
-  parentRow(forRow:) 

Instance Method

# parentRow(forRow:)

Returns the index of the parent of a given row.

macOS

``` source
@MainActor
func parentRow(forRow rowIndex: Int) -> Int
```

## Parameters 

`rowIndex`  

The index of a row in the receiver.

Important

Raises an `NSRangeException` if `rowIndex` is less than `0` or greater than or equal to the number of rows.

## Return Value

The index of the parent of the row at `rowIndex`. If the row at `rowIndex` is a root row, returns `-1`.

## See Also

### Obtaining Row Information

var numberOfRows: Int

The number of rows in the rule editor.

func row(forDisplayValue: Any) -> Int

Returns the index of the row containing a given value.

func rowType(forRow: Int) -> NSRuleEditor.RowType

Returns the type of a given row.

enum RowType

Specifies a type for row types.

func subrowIndexes(forRow: Int) -> IndexSet

Returns the immediate subrows of a given row.

