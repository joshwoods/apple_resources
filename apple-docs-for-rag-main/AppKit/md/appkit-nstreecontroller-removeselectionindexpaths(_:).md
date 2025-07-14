

- AppKit
- NSTreeController
-  removeSelectionIndexPaths(\_:) 

Instance Method

# removeSelectionIndexPaths(\_:)

Removes the objects at the specified `indexPaths` from the tree controller’s current selection, returning true if the selection was changed.

macOS

``` source
func removeSelectionIndexPaths(_ indexPaths: [IndexPath]) -> Bool
```

## Discussion

Attempting to change the selection may cause a `commitEditing` message which fails, thus denying the selection change.

## See Also

### Managing Selections

var selectsInsertedObjects: Bool

A Boolean value that indicates whether the tree controller automatically selects objects as they are inserted.

func addSelectionIndexPaths([IndexPath]) -> Bool

Adds the objects at the specified `indexPaths` in the tree controller’s content to the current selection.

var avoidsEmptySelection: Bool

A Boolean value that indicates whether the tree controller requires the content array to attempt to maintain a selection at all times, avoiding an empty selection.

var preservesSelection: Bool

A Boolean value that indicates whether the tree controller will attempt to preserve the current selection when the content changes.

var alwaysUsesMultipleValuesMarker: Bool

A Boolean value that indicates whether the tree controller always returns the multiple values marker when multiple objects are selected, even if the selected items have the same value.

