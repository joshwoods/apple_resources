

- AppKit
- NSBrowser
-  selectRowIndexes(\_:inColumn:) 

Instance Method

# selectRowIndexes(\_:inColumn:)

Specifies the selected rows in a given column of the browser.

macOS 10.5+

``` source
@MainActor
func selectRowIndexes(
    _ indexes: IndexSet,
    inColumn column: Int
)
```

## Parameters 

`indexes`  

Rows to be selected in column `columnIndex`.

`column`  

Column in which to select rows `rowIndexes`.

## See Also

### Managing Selection Behavior

var allowsBranchSelection: Bool

A Boolean that indicates whether the user can select branch items.

var allowsEmptySelection: Bool

A Boolean that indicates whether there can be nothing selected.

var allowsMultipleSelection: Bool

A Boolean that indicates whether the user can select multiple items.

func selectedRowIndexes(inColumn: Int) -> IndexSet?

Provides the indexes of the selected rows in a given column of the browser.

var allowsTypeSelect: Bool

A Boolean that indicates whether the browser allows keystroke-based selection (type select).

