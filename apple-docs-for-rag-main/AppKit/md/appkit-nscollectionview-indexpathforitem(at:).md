

- AppKit
- NSCollectionView
-  indexPathForItem(at:) 

Instance Method

# indexPathForItem(at:)

Returns the index path of the item at the specified point.

macOS 10.11+

``` source
@MainActor
func indexPathForItem(at point: NSPoint) -> IndexPath?
```

## Parameters 

`point`  

The point in the collection view’s bounds that you want to test.

## Return Value

The item at the specified point or `nil` if no item was found at that point.

## Discussion

This method uses the available layout attributes to determine which item is at the specified point. If more than one item is at the point, this method returns only the top-most item. This method ignores the opacity of the item, so items that are fully transparent are still returned by this method. Hidden items are never returned.

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

func indexPath(for: NSCollectionViewItem) -> IndexPath?

Returns the index path of the specified item.

func item(at: IndexPath) -> NSCollectionViewItem?

Returns the item associated with the specified index path.

func supplementaryView(forElementKind: NSCollectionView.SupplementaryElementKind, at: IndexPath) -> (any NSView &amp; NSCollectionViewElement)?

Returns the supplementary view associated with the specified index path.

func scrollToItems(at: Set&lt;IndexPath>, scrollPosition: NSCollectionView.ScrollPosition)

Scrolls the collection view contents until the specified items are visible.

