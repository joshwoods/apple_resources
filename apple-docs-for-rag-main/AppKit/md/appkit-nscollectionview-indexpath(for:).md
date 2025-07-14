

- AppKit
- NSCollectionView
-  indexPath(for:) 

Instance Method

# indexPath(for:)

Returns the index path of the specified item.

macOS 10.11+

``` source
@MainActor
func indexPath(for item: NSCollectionViewItem) -> IndexPath?
```

## Parameters 

`item`  

The item whose index path you want to know.

## Return Value

The item’s index path or `nil` if the item is not in the collection view.

## See Also

### Locating Items and Views

func visibleItems() -> [NSCollectionViewItem]

Returns an array of the actively managed items in the collection view.

func indexPathsForVisibleItems() -> Set&lt;IndexPath>

Returns the index paths of the currently active items.

func visibleSupplementaryViews(ofKind: NSCollectionView.SupplementaryElementKind) -> [any NSView &amp; NSCollectionViewElement]

Returns an array of the actively managed supplementary views in the collection view.

func indexPathsForVisibleSupplementaryElements(ofKind: NSCollectionView.SupplementaryElementKind) -> Set&lt;IndexPath>

Returns the index paths of the currently active supplementary views.

func indexPathForItem(at: NSPoint) -> IndexPath?

Returns the index path of the item at the specified point.

func item(at: IndexPath) -> NSCollectionViewItem?

Returns the item associated with the specified index path.

func supplementaryView(forElementKind: NSCollectionView.SupplementaryElementKind, at: IndexPath) -> (any NSView &amp; NSCollectionViewElement)?

Returns the supplementary view associated with the specified index path.

func scrollToItems(at: Set&lt;IndexPath>, scrollPosition: NSCollectionView.ScrollPosition)

Scrolls the collection view contents until the specified items are visible.

