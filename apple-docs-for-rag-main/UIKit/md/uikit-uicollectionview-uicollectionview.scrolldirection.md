

- UIKit
- UICollectionView
-  UICollectionView.ScrollDirection 

Enumeration

# UICollectionView.ScrollDirection

Constants that indicate the direction of scrolling for the layout.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum ScrollDirection
```

## Topics

### Constants

case vertical

The layout scrolls content vertically.

case horizontal

The layout scrolls content horizontally.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Scrolling an item into view

func scrollToItem(at: IndexPath, at: UICollectionView.ScrollPosition, animated: Bool)

Scrolls the collection view contents until the specified item is visible.

struct ScrollPosition

Constants that indicate how to scroll an item into the visible portion of the collection view.

