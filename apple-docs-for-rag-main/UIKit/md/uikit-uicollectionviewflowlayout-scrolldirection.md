

- UIKit
- UICollectionViewFlowLayout
-  scrollDirection 

Instance Property

# scrollDirection

The scroll direction of the grid.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var scrollDirection: UICollectionView.ScrollDirection { get set }
```

## Discussion

The grid layout scrolls along one axis only, either horizontally or vertically. For the non scrolling axis, the width of the collection view in that dimension serves as starting width of the content.

The default value of this property is UICollectionView.ScrollDirection.vertical.

## See Also

### Configuring the scroll direction

enum ScrollDirection

Constants that indicate the direction of scrolling for the layout.

