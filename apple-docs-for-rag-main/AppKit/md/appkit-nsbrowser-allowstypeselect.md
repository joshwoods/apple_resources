

- AppKit
- NSBrowser
-  allowsTypeSelect 

Instance Property

# allowsTypeSelect

A Boolean that indicates whether the browser allows keystroke-based selection (type select).

macOS 10.5+

``` source
@MainActor
var allowsTypeSelect: Bool { get set }
```

## Discussion

When the value of this property is true, the browser allows keystroke-based selection. The default value of this property is true.

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

func selectRowIndexes(IndexSet, inColumn: Int)

Specifies the selected rows in a given column of the browser.

