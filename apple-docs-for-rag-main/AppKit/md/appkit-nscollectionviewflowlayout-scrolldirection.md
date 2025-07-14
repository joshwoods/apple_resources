

- AppKit
- NSCollectionViewFlowLayout
-  scrollDirection 

Instance Property

# scrollDirection

The scroll direction of the layout.

macOS 10.11+

``` source
@MainActor
var scrollDirection: NSCollectionView.ScrollDirection { get set }
```

## Discussion

The flow layout scrolls along one axis only, either horizontally or vertically. When the scroll direction is NSCollectionView.ScrollDirection.vertical, the width of the content never exceeds the width of the collection view itself but the height grows as needed to accommodate the current items. When the scroll direction is NSCollectionView.ScrollDirection.horizontal, the height never exceeds the height of the collection view but the width grows as needed.

The default value of this property is NSCollectionView.ScrollDirection.vertical.

