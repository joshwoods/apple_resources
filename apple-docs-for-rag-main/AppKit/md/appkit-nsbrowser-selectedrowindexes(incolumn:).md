

- AppKit
- NSBrowser
-  selectedRowIndexes(inColumn:) 

Instance Method

# selectedRowIndexes(inColumn:)

Provides the indexes of the selected rows in a given column of the browser.

macOS 10.5+

``` source
@MainActor
func selectedRowIndexes(inColumn column: Int) -> IndexSet?
```

## Parameters 

`column`  

The column whose selected rows are provided.

## Return Value

Rows selected in column `columnIndex`.

## See Also

### Managing Selection Behavior

var allowsBranchSelection: Bool

A Boolean that indicates whether the user can select branch items.

var allowsEmptySelection: Bool

A Boolean that indicates whether there can be nothing selected.

var allowsMultipleSelection: Bool

A Boolean that indicates whether the user can select multiple items.

func selectRowIndexes(IndexSet, inColumn: Int)

Specifies the selected rows in a given column of the browser.

var allowsTypeSelect: Bool

A Boolean that indicates whether the browser allows keystroke-based selection (type select).

