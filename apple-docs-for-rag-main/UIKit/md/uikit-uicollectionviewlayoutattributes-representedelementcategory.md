

- UIKit
- UICollectionViewLayoutAttributes
-  representedElementCategory 

Instance Property

# representedElementCategory

The type of the item.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var representedElementCategory: UICollectionView.ElementCategory { get }
```

## Discussion

You can use the value in this property to distinguish whether the layout attributes are intended for a cell, supplementary view, or decoration view.

## See Also

### Identifying the referenced item

var indexPath: IndexPath

The index path of the item in the collection view.

var representedElementKind: String?

The layout-specific identifier for the target view.

enum ElementCategory

Constants specifying the type of view.

