

- AppKit
- NSBrowser
-  allowsMultipleSelection 

Instance Property

# allowsMultipleSelection

A Boolean that indicates whether the user can select multiple items.

macOS

``` source
@MainActor
var allowsMultipleSelection: Bool { get set }
```

## Discussion

When the value of this property is true, the browser allows the user to select multiple items at once.

## See Also

### Managing Selection Behavior

var allowsBranchSelection: Bool

A Boolean that indicates whether the user can select branch items.

var allowsEmptySelection: Bool

A Boolean that indicates whether there can be nothing selected.

func selectedRowIndexes(inColumn: Int) -> IndexSet?

Provides the indexes of the selected rows in a given column of the browser.

func selectRowIndexes(IndexSet, inColumn: Int)

Specifies the selected rows in a given column of the browser.

var allowsTypeSelect: Bool

A Boolean that indicates whether the browser allows keystroke-based selection (type select).

