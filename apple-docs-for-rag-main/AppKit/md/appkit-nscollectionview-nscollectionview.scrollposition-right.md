

- AppKit
- NSCollectionView
- NSCollectionView.ScrollPosition
-  right 

Type Property

# right

Scroll so that the right edge of the selected items’ bounding box is adjacent to the right edge of the collection view’s bounds. This option must not be combined with the left, centeredHorizontally, leadingEdge, trailingEdge, or nearestVerticalEdge options, but may be combined with other options.

macOS

``` source
static var right: NSCollectionView.ScrollPosition { get }
```

## See Also

### Constants

static var top: NSCollectionView.ScrollPosition

Scroll so that the top edge of the selected items’ bounding box is adjacent to the top edge of the collection view’s bounds. This option must not be combined with the centeredVertically, bottom, and nearestHorizontalEdge options, but may be combined with other options.

static var centeredVertically: NSCollectionView.ScrollPosition

Scroll so that the bounding box of the selected items is centered vertically in the collection view’s bounds. This option must not be combined with the top, bottom, or nearestHorizontalEdge options, but may be combined with other options.

static var bottom: NSCollectionView.ScrollPosition

Scroll so that the bottom edge of the bounding box is adjacent to the bottom of the collection view’s bounds. This option must not be combined with the top, centeredVertically, or nearestHorizontalEdge options, but may be combined with other options.

static var nearestHorizontalEdge: NSCollectionView.ScrollPosition

Scroll so that the bounding box is adjacent to the nearest edge (top or bottom) of the collection view. This option must not be combined with the top, centeredVertically, or bottom options, but may be combined with other options.

static var left: NSCollectionView.ScrollPosition

Scroll so that the left edge of the selected items’ bounding box is adjacent to the left edge of the collection view’s bounds. This option must not be combined with the centeredHorizontally, right, leadingEdge, trailingEdge, or nearestVerticalEdge options, but may be combined with other options.

static var centeredHorizontally: NSCollectionView.ScrollPosition

Scroll so that the selected items’ bounding box is centered horizontally in the collection view’s bounds. This option must not be combined with the left, right, leadingEdge, trailingEdge, or nearestVerticalEdge options, but may be combined with other options.

static var leadingEdge: NSCollectionView.ScrollPosition

Scroll so that the leading edge of the selected items’ bounding box is adjacent to the leading edge of the collection view’s bounds. Use this option to support both left-to-right and right-to-left layouts appropriately. This option must not be combined with the left, centeredHorizontally, right, trailingEdge, or nearestVerticalEdge options, but may be combined with other options.

static var trailingEdge: NSCollectionView.ScrollPosition

Scroll so that the trailing edge of the selected items’ bounding box is adjacent to the trailing edge of the collection view’s bounds. Use this option to support both left-to-right and right-to-left layouts appropriately. This option must not be combined with the left, centeredHorizontally, right, leadingEdge, or nearestVerticalEdge options, but may be combined with other options.

static var nearestVerticalEdge: NSCollectionView.ScrollPosition

Scroll so that the bounding box is adjacent to the nearest edge (leading or trailing) of the collection view. Use this option to support both left-to-right and right-to-left layouts appropriately. This option must not be combined with the left, centeredHorizontally, right, leadingEdge, or trailingEdge options, but may be combined with other options.

