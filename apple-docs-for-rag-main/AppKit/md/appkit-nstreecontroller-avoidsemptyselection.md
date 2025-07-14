

- AppKit
- NSTreeController
-  avoidsEmptySelection 

Instance Property

# avoidsEmptySelection

A Boolean value that indicates whether the tree controller requires the content array to attempt to maintain a selection at all times, avoiding an empty selection.

macOS

``` source
var avoidsEmptySelection: Bool { get set }
```

## Discussion

When the value of this property is true, the tree controller maintains a selection unless there are no objects in the content. The default value is true. This property is observable using key-value observing.

## See Also

### Managing Selections

var selectsInsertedObjects: Bool

A Boolean value that indicates whether the tree controller automatically selects objects as they are inserted.

func addSelectionIndexPaths([IndexPath]) -> Bool

Adds the objects at the specified `indexPaths` in the tree controller’s content to the current selection.

func removeSelectionIndexPaths([IndexPath]) -> Bool

Removes the objects at the specified `indexPaths` from the tree controller’s current selection, returning true if the selection was changed.

var preservesSelection: Bool

A Boolean value that indicates whether the tree controller will attempt to preserve the current selection when the content changes.

var alwaysUsesMultipleValuesMarker: Bool

A Boolean value that indicates whether the tree controller always returns the multiple values marker when multiple objects are selected, even if the selected items have the same value.

