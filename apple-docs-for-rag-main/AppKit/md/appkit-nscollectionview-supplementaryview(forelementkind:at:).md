

- AppKit
- NSCollectionView
-  supplementaryView(forElementKind:at:) 

Instance Method

# supplementaryView(forElementKind:at:)

Returns the supplementary view associated with the specified index path.

macOS 10.11+

``` source
@MainActor
func supplementaryView(
    forElementKind elementKind: NSCollectionView.SupplementaryElementKind,
    at indexPath: IndexPath
) -> (any NSView & NSCollectionViewElement)?
```

## Parameters 

`elementKind`  

The kind of the supplementary views you want returned. The layout object defines the kinds of supplementary views it supports. This parameter must not be `nil`.

`indexPath`  

The index path whose supplementary view you want.

## Return Value

The view for the specified index path or `nil` if no view is available.

## Discussion

For efficiency, the collection view does not create supplementary views until they are needed. Typically, views are created only when they need to be displayed onscreen. If the collection view does not currently have a supplementary view for the specified index path, because that view would be positioned offscreen, this method returns `nil`.

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

func item(at: IndexPath) -> NSCollectionViewItem?

Returns the item associated with the specified index path.

func scrollToItems(at: Set&lt;IndexPath>, scrollPosition: NSCollectionView.ScrollPosition)

Scrolls the collection view contents until the specified items are visible.

