

- UIKit
- UICollectionView
-  allowsSelection 

Instance Property

# allowsSelection

A Boolean value that indicates whether users can select items in the collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var allowsSelection: Bool { get set }
```

## Discussion

If the value of this property is true (the default), users can select items. If you want more fine-grained control over the selection of items, you must provide a delegate object and implement the appropriate methods of the UICollectionViewDelegate protocol.

## See Also

### Selecting cells

var indexPathsForSelectedItems: [IndexPath]?

The index paths for the selected items.

func selectItem(at: IndexPath?, animated: Bool, scrollPosition: UICollectionView.ScrollPosition)

Selects the item at the specified index path and optionally scrolls it into view.

func deselectItem(at: IndexPath, animated: Bool)

Deselects the item at the specified index.

var allowsMultipleSelection: Bool

A Boolean value that determines whether users can select more than one item in the collection view.

var allowsSelectionDuringEditing: Bool

A Boolean value that determines whether users can select cells while the collection view is in editing mode.

var allowsMultipleSelectionDuringEditing: Bool

A Boolean value that controls whether users can select more than one cell simultaneously in editing mode.

var selectionFollowsFocus: Bool

A Boolean value that triggers an automatic selection when focus moves to a cell.

