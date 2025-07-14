

- AppKit
- NSCollectionView
-  visibleSupplementaryViews(ofKind:) 

Instance Method

# visibleSupplementaryViews(ofKind:)

Returns an array of the actively managed supplementary views in the collection view.

macOS 10.11+

``` source
@MainActor
func visibleSupplementaryViews(ofKind elementKind: NSCollectionView.SupplementaryElementKind) -> [any NSView & NSCollectionViewElement]
```

## Parameters 

`elementKind`  

The kind of the supplementary views you want returned. The layout object defines the kinds of supplementary views it supports. This parameter must not be `nil`.

## Return Value

An array of view objects. The returned array may be empty.

## Discussion

The views returned by this method represent the ones that are active and are currently being managed by the collection view. The array may contain supplementary views that are outside of the collection view’s actual visible rectangle. For example, it might contain views that were recently visible but have since been scrolled out of the visible rectangle. To test whether a view is actually visible, check to see if its frame rectangle intersects the visibleRect of the collection view.

## See Also

### Locating Items and Views

func visibleItems() -> [NSCollectionViewItem]

Returns an array of the actively managed items in the collection view.

func indexPathsForVisibleItems() -> Set&lt;IndexPath>

Returns the index paths of the currently active items.

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

