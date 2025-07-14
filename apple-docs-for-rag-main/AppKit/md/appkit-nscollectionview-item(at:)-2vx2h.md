

- AppKit
- NSCollectionView
-  item(at:) 

Instance Method

# item(at:)

Returns the item associated with the specified index path.

macOS 10.11+

``` source
@MainActor
func item(at indexPath: IndexPath) -> NSCollectionViewItem?
```

## Parameters 

`indexPath`  

The index path whose item you want.

## Return Value

The item for the specified index path or `nil` if no item is available.

## Discussion

For efficiency, the collection view does not create items until they are needed, and usually it creates them only when they need to be displayed onscreen. If the collection view does not currently have an item for the specified index path, because that item would be positioned offscreen, this method returns `nil`.

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

func indexPathForItem(at: NSPoint) -> IndexPath?

Returns the index path of the item at the specified point.

func supplementaryView(forElementKind: NSCollectionView.SupplementaryElementKind, at: IndexPath) -> (any NSView &amp; NSCollectionViewElement)?

Returns the supplementary view associated with the specified index path.

func scrollToItems(at: Set&lt;IndexPath>, scrollPosition: NSCollectionView.ScrollPosition)

Scrolls the collection view contents until the specified items are visible.

