

- AppKit
- NSCollectionView
-  indexPathsForVisibleItems() 

Instance Method

# indexPathsForVisibleItems()

Returns the index paths of the currently active items.

macOS 10.11+

``` source
@MainActor
func indexPathsForVisibleItems() -> Set
```

## Return Value

The set of NSIndexPath objects corresponding to the currently visible items.

## Discussion

The index paths returned by this method belong to items that are active and currently being managed by the collection view. As a result, the returned set may include index paths for items that are outside of the collection view’s actual visible rectangle. For example, it may contain index paths for items that were recently visible but have since been scrolled out of view. To test whether an item is visible, check to see if its frame rectangle intersects the visibleRect of the collection view.

## See Also

### Locating Items and Views

func visibleItems() -> [NSCollectionViewItem]

Returns an array of the actively managed items in the collection view.

func visibleSupplementaryViews(ofKind: NSCollectionView.SupplementaryElementKind) -> [any NSView &amp; NSCollectionViewElement]

Returns an array of the actively managed supplementary views in the collection view.

func indexPathsForVisibleSupplementaryElements(ofKind: NSCollectionView.SupplementaryElementKind) -> Set&lt;IndexPath>

Returns the index paths of the currently active supplementary views.

func indexPath(for: NSCollectionViewItem) -> IndexPath?

Returns the index path of the specified item.

func indexPathForItem(at: NSPoint) -> IndexPath?

Returns the index path of the item at the specified point.

func item(at: IndexPath) -> NSCollectionViewItem?

Returns the item associated with the specified index path.

func supplementaryView(forElementKind: NSCollectionView.SupplementaryElementKind, at: IndexPath) -> (any NSView &amp; NSCollectionViewElement)?

Returns the supplementary view associated with the specified index path.

func scrollToItems(at: Set&lt;IndexPath>, scrollPosition: NSCollectionView.ScrollPosition)

Scrolls the collection view contents until the specified items are visible.

