

- AppKit
- NSCollectionView
-  selectionIndexPaths 

Instance Property

# selectionIndexPaths

The set of index paths representing the currently selected items.

macOS 10.11+

``` source
@MainActor
var selectionIndexPaths: Set { get set }
```

## Discussion

This property reflects the index paths of the currently selected items, where each index path contains a section number and an index number for the item in that section. This property is updated automatically when the user selects items interactively. You can also change the selection programmatically by assigning a new value to this property. To animate changes to the selection, call this method on the collection view’s animator() proxy object instead.

It is a programmer error to specify an index path that does not refer to a valid item in the data source. If you specify an invalid index path, this method raises an exception.

This property is key-value observable. Other methods that modify the selection automatically update this property.

## See Also

### Managing the Selection

var isSelectable: Bool

A Boolean value that indicates whether the user may select items in the collection view.

var allowsMultipleSelection: Bool

A Boolean value that indicates whether the user may select more than one item in the collection view.

var allowsEmptySelection: Bool

A Boolean value indicating whether the collection view may have no selected items.

func selectAll(Any?)

Selects all items in the collection view, if doing so is possible.

func deselectAll(Any?)

Deselects all items in the collection view.

func selectItems(at: Set&lt;IndexPath>, scrollPosition: NSCollectionView.ScrollPosition)

Adds the specified items to the current selection and optionally scrolls the items into position.

func deselectItems(at: Set&lt;IndexPath>)

Removes the specified items from the current selection.

