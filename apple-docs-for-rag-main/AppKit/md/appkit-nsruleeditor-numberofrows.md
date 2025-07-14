

- AppKit
- NSRuleEditor
-  numberOfRows 

Instance Property

# numberOfRows

The number of rows in the rule editor.

macOS

``` source
@MainActor
var numberOfRows: Int { get }
```

## See Also

### Obtaining Row Information

func parentRow(forRow: Int) -> Int

Returns the index of the parent of a given row.

func row(forDisplayValue: Any) -> Int

Returns the index of the row containing a given value.

func rowType(forRow: Int) -> NSRuleEditor.RowType

Returns the type of a given row.

enum RowType

Specifies a type for row types.

func subrowIndexes(forRow: Int) -> IndexSet

Returns the immediate subrows of a given row.

