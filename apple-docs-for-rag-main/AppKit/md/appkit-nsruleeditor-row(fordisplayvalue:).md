

- AppKit
- NSRuleEditor
-  row(forDisplayValue:) 

Instance Method

# row(forDisplayValue:)

Returns the index of the row containing a given value.

macOS

``` source
@MainActor
func row(forDisplayValue displayValue: Any) -> Int
```

## Parameters 

`displayValue`  

The display value (string, view, or menu item) of an item in the receiver. This value must not be `nil`.

Important

Raises `NSInvalidArgumentException` if `displayValue` is `nil`.

## Return Value

The index of the row containing `displayValue`, or `NSNotFound`.

## Discussion

This method searches each row via pointer equality for the given display value, which may be present as an alternative in a popup menu for that row.

## See Also

### Obtaining Row Information

var numberOfRows: Int

The number of rows in the rule editor.

func parentRow(forRow: Int) -> Int

Returns the index of the parent of a given row.

func rowType(forRow: Int) -> NSRuleEditor.RowType

Returns the type of a given row.

enum RowType

Specifies a type for row types.

func subrowIndexes(forRow: Int) -> IndexSet

Returns the immediate subrows of a given row.

