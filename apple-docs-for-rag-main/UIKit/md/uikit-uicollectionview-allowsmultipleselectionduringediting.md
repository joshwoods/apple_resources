

- UIKit
- UICollectionView
-  allowsMultipleSelectionDuringEditing 

Instance Property

# allowsMultipleSelectionDuringEditing

A Boolean value that controls whether users can select more than one cell simultaneously in editing mode.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var allowsMultipleSelectionDuringEditing: Bool { get set }
```

## Discussion

The default value is false.

## See Also

### Selecting cells

var indexPathsForSelectedItems: [IndexPath]?

The index paths for the selected items.

func selectItem(at: IndexPath?, animated: Bool, scrollPosition: UICollectionView.ScrollPosition)

Selects the item at the specified index path and optionally scrolls it into view.

func deselectItem(at: IndexPath, animated: Bool)

Deselects the item at the specified index.

var allowsSelection: Bool

A Boolean value that indicates whether users can select items in the collection view.

var allowsMultipleSelection: Bool

A Boolean value that determines whether users can select more than one item in the collection view.

var allowsSelectionDuringEditing: Bool

A Boolean value that determines whether users can select cells while the collection view is in editing mode.

var selectionFollowsFocus: Bool

A Boolean value that triggers an automatic selection when focus moves to a cell.

