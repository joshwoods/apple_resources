

- UIKit
- UICollectionView
-  selectItem(at:animated:scrollPosition:) 

Instance Method

# selectItem(at:animated:scrollPosition:)

Selects the item at the specified index path and optionally scrolls it into view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func selectItem(
    at indexPath: IndexPath?,
    animated: Bool,
    scrollPosition: UICollectionView.ScrollPosition
)
```

## Parameters 

`indexPath`  

The index path of the item to select. Specifying `nil` for this parameter clears the current selection.

`animated`  

Specify true to animate the change in the selection or false to make the change without animating it.

`scrollPosition`  

An option that specifies where the item should be positioned when scrolling finishes. For a list of possible values, see UICollectionView.ScrollPosition.

## Discussion

If the allowsSelection property is false, calling this method has no effect. If there’s an existing selection with a different index path and the allowsMultipleSelection property is false, calling this method replaces the previous selection.

This method doesn’t cause any selection-related delegate methods to be called.

## See Also

### Selecting cells

var indexPathsForSelectedItems: [IndexPath]?

The index paths for the selected items.

func deselectItem(at: IndexPath, animated: Bool)

Deselects the item at the specified index.

var allowsSelection: Bool

A Boolean value that indicates whether users can select items in the collection view.

var allowsMultipleSelection: Bool

A Boolean value that determines whether users can select more than one item in the collection view.

var allowsSelectionDuringEditing: Bool

A Boolean value that determines whether users can select cells while the collection view is in editing mode.

var allowsMultipleSelectionDuringEditing: Bool

A Boolean value that controls whether users can select more than one cell simultaneously in editing mode.

var selectionFollowsFocus: Bool

A Boolean value that triggers an automatic selection when focus moves to a cell.

