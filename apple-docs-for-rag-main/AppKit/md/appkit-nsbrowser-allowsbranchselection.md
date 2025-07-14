

- AppKit
- NSBrowser
-  allowsBranchSelection 

Instance Property

# allowsBranchSelection

A Boolean that indicates whether the user can select branch items.

macOS

``` source
@MainActor
var allowsBranchSelection: Bool { get set }
```

## Discussion

When the value of this property is true, the user can select branch items when multiple selection is enabled.

## See Also

### Managing Selection Behavior

var allowsEmptySelection: Bool

A Boolean that indicates whether there can be nothing selected.

var allowsMultipleSelection: Bool

A Boolean that indicates whether the user can select multiple items.

func selectedRowIndexes(inColumn: Int) -> IndexSet?

Provides the indexes of the selected rows in a given column of the browser.

func selectRowIndexes(IndexSet, inColumn: Int)

Specifies the selected rows in a given column of the browser.

var allowsTypeSelect: Bool

A Boolean that indicates whether the browser allows keystroke-based selection (type select).

