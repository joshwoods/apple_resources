

- AppKit
- NSCollectionView
-  selectItems(at:scrollPosition:) 

Instance Method

# selectItems(at:scrollPosition:)

Adds the specified items to the current selection and optionally scrolls the items into position.

macOS 10.11+

``` source
@MainActor
func selectItems(
    at indexPaths: Set,
    scrollPosition: NSCollectionView.ScrollPosition
)
```

## Parameters 

`indexPaths`  

The index paths of the items you want to select.

`scrollPosition`  

The options for scrolling the newly selected items into view. You may combine one vertical and one horizontal scrolling option when calling this method. Specifying more than one option for either the vertical or horizontal directions raises an exception.

## Discussion

Use this method to extend the current selection. If you want to animate the selection of the new items, call this method on the collection view’s animator() proxy object instead. This method does not call any methods of the delegate object when making the selection.

## See Also

### Managing the Selection

var isSelectable: Bool

A Boolean value that indicates whether the user may select items in the collection view.

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

func deselectItems(at: Set&lt;IndexPath>)

Removes the specified items from the current selection.

