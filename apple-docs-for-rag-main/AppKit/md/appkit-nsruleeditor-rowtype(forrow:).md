

- AppKit
- NSRuleEditor
-  rowType(forRow:) 

Instance Method

# rowType(forRow:)

Returns the type of a given row.

macOS

``` source
@MainActor
func rowType(forRow rowIndex: Int) -> NSRuleEditor.RowType
```

## Parameters 

`rowIndex`  

The index of a row in the receiver.

Important

Raises an `NSRangeException` if `rowIndex` is less than `0` or greater than or equal to the number of rows.

## Return Value

The type of the row at `rowIndex`.

## See Also

### Obtaining Row Information

var numberOfRows: Int

The number of rows in the rule editor.

func parentRow(forRow: Int) -> Int

Returns the index of the parent of a given row.

func row(forDisplayValue: Any) -> Int

Returns the index of the row containing a given value.

enum RowType

Specifies a type for row types.

func subrowIndexes(forRow: Int) -> IndexSet

Returns the immediate subrows of a given row.

