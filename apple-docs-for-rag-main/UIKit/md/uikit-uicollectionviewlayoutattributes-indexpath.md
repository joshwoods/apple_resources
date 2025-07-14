

- UIKit
- UICollectionViewLayoutAttributes
-  indexPath 

Instance Property

# indexPath

The index path of the item in the collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var indexPath: IndexPath { get set }
```

## Discussion

The index path contains the index of the section and the index of the item within that section. These two values uniquely identify the position of the corresponding item in the collection view.

## See Also

### Identifying the referenced item

var representedElementKind: String?

The layout-specific identifier for the target view.

var representedElementCategory: UICollectionView.ElementCategory

The type of the item.

enum ElementCategory

Constants specifying the type of view.

