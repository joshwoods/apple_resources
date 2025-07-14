

- UIKit
- UICollectionViewLayoutAttributes
-  representedElementKind 

Instance Property

# representedElementKind

The layout-specific identifier for the target view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var representedElementKind: String? { get }
```

## Discussion

You can use the value in this property to identify the specific purpose of the supplementary or decoration view associated with the attributes. This property is `nil` if the representedElementCategory property contains the value UICollectionView.ElementCategory.cell.

## See Also

### Identifying the referenced item

var indexPath: IndexPath

The index path of the item in the collection view.

var representedElementCategory: UICollectionView.ElementCategory

The type of the item.

enum ElementCategory

Constants specifying the type of view.

