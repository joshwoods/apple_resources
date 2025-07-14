

- AppKit
- NSCollectionView
-  scrollToItems(at:scrollPosition:) 

Instance Method

# scrollToItems(at:scrollPosition:)

Scrolls the collection view contents until the specified items are visible.

macOS 10.11+

``` source
@MainActor
func scrollToItems(
    at indexPaths: Set,
    scrollPosition: NSCollectionView.ScrollPosition
)
```

## Parameters 

`indexPaths`  

The index paths of the items. The layout attributes of these items define the bounding box that needs to be scrolled onscreen.

`scrollPosition`  

The options for scrolling the bounding box of the specified items into view. You may combine one vertical and one horizontal scrolling option when calling this method. Specifying more than one option for either the vertical or horizontal directions raises an exception.

## Discussion

To animate the scrolling operation, call this method on the collection view’s animator() proxy object instead.

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

func supplementaryView(forElementKind: NSCollectionView.SupplementaryElementKind, at: IndexPath) -> (any NSView &amp; NSCollectionViewElement)?

Returns the supplementary view associated with the specified index path.

