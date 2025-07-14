

- AppKit
- NSCollectionView
-  isSelectable 

Instance Property

# isSelectable

A Boolean value that indicates whether the user may select items in the collection view.

macOS 10.5+

``` source
@MainActor
var isSelectable: Bool { get set }
```

## Discussion

The value of this property is true when the collection view allows the user to select items, or false when it does not. You can set selections programmatically regardless of this setting.

The default value of this property is false. Changing the value from true to false removes the current selection if there is one.

## See Also

### Managing the Selection

var allowsMultipleSelection: Bool

A Boolean value that indicates whether the user may select more than one item in the collection view.

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

