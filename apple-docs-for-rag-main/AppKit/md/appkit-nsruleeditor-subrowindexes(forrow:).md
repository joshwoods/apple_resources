

- AppKit
- NSRuleEditor
-  subrowIndexes(forRow:) 

Instance Method

# subrowIndexes(forRow:)

Returns the immediate subrows of a given row.

macOS

``` source
@MainActor
func subrowIndexes(forRow rowIndex: Int) -> IndexSet
```

## Parameters 

`rowIndex`  

The index of a row in the receiver, or `-1` to get the top-level rows.

Important

Raises an `NSRangeException` if `rowIndex` is less than `-1` or greater than or equal to the number of rows.

## Return Value

The immediate subrows of the row at `rowIndex`.

## Discussion

Rows are numbered starting at `0`.

## See Also

### Obtaining Row Information

var numberOfRows: Int

The number of rows in the rule editor.

func parentRow(forRow: Int) -> Int

Returns the index of the parent of a given row.

func row(forDisplayValue: Any) -> Int

Returns the index of the row containing a given value.

func rowType(forRow: Int) -> NSRuleEditor.RowType

Returns the type of a given row.

enum RowType

Specifies a type for row types.

