

- AppKit
- NSCollectionView
-  allowsMultipleSelection 

Instance Property

# allowsMultipleSelection

A Boolean value that indicates whether the user may select more than one item in the collection view.

macOS 10.5+

``` source
@MainActor
var allowsMultipleSelection: Bool { get set }
```

## Discussion

The value of this property is true if the collection view supports the selection of more than one item at a time. The default value of this property is false. Changing the value from true to false reduces the current selection to the first item in the selected group.

## See Also

### Managing the Selection

var isSelectable: Bool

A Boolean value that indicates whether the user may select items in the collection view.

var allowsEmptySelection: Bool

A Boolean value indicating whether the collection view may have no selected items.

var selectionIndexPaths: Set&lt;IndexPath>

The set of index paths representing the currently selected items.

func selectAll(Any?)

Selects all items in the collection view, if doing so is possible.

func deselectAll(Any?)

Deselects all items in the collection view.

func selectItems(at: Set&lt;IndexPath>, scrollPosition: NSCollectionView.ScrollPosition)

Adds the specified items to the current selection and optionally scrolls the items into position.

func deselectItems(at: Set&lt;IndexPath>)

Removes the specified items from the current selection.

