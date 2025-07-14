

- UIKit
- UICollectionView
-  UICollectionView.ScrollPosition 

Structure

# UICollectionView.ScrollPosition

Constants that indicate how to scroll an item into the visible portion of the collection view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct ScrollPosition
```

## Topics

### Constants

static var top: UICollectionView.ScrollPosition

Scroll so that the item is positioned at the top of the collection view’s bounds.

static var centeredVertically: UICollectionView.ScrollPosition

Scroll so that the item is centered vertically in the collection view.

static var bottom: UICollectionView.ScrollPosition

Scroll so that the item is positioned at the bottom of the collection view’s bounds.

static var left: UICollectionView.ScrollPosition

Scroll so that the item is positioned at the left edge of the collection view’s bounds.

static var centeredHorizontally: UICollectionView.ScrollPosition

Scroll so that the item is centered horizontally in the collection view.

static var right: UICollectionView.ScrollPosition

Scroll so that the item is positioned at the right edge of the collection view’s bounds.

### Initializers

init(rawValue: UInt)

Creates a scroll-position structure with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Scrolling an item into view

func scrollToItem(at: IndexPath, at: UICollectionView.ScrollPosition, animated: Bool)

Scrolls the collection view contents until the specified item is visible.

enum ScrollDirection

Constants that indicate the direction of scrolling for the layout.

