

- AppKit
- NSCollectionView
-  allowsEmptySelection 

Instance Property

# allowsEmptySelection

A Boolean value indicating whether the collection view may have no selected items.

macOS 10.11+

``` source
@MainActor
var allowsEmptySelection: Bool { get set }
```

## Discussion

The default value of this property is true, which allows the collection view to have no selected items. Setting this property to false causes the collection view to always leave at least one item selected.

## See Also

### Managing the Selection

var isSelectable: Bool

A Boolean value that indicates whether the user may select items in the collection view.

var allowsMultipleSelection: Bool

A Boolean value that indicates whether the user may select more than one item in the collection view.

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

