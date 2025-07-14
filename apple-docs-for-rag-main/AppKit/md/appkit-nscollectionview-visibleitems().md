

- AppKit
- NSCollectionView
-  visibleItems() 

Instance Method

# visibleItems()

Returns an array of the actively managed items in the collection view.

macOS 10.11+

``` source
@MainActor
func visibleItems() -> [NSCollectionViewItem]
```

## Return Value

An array of NSCollectionViewItem objects. The returned array may be empty.

## Discussion

The items returned by this method represent the ones that are active and currently being managed by the collection view. This array may contain items that are outside of the collection view’s actual visible rectangle. For example, it may contain items that were recently visible but have since been scrolled out of view. To test whether an item is actually visible, check to see if its frame rectangle intersects the visibleRect of the collection view.

## See Also

### Locating Items and Views

func indexPathsForVisibleItems() -> Set&lt;IndexPath>

Returns the index paths of the currently active items.

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

