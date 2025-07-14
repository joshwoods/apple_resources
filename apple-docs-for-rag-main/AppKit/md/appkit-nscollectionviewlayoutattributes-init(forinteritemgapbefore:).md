

- AppKit
- NSCollectionViewLayoutAttributes
-  init(forInterItemGapBefore:) 

Initializer

# init(forInterItemGapBefore:)

Creates and returns a layout attributes object for an inter-item gap view at the specified index path.

macOS 10.11+

``` source
@MainActor
convenience init(forInterItemGapBefore indexPath: IndexPath)
```

## Parameters 

`indexPath`  

The index path at which to insert the gap view. The gap is placed after the item specified by the index path. This parameter must contain a valid value.

## Return Value

A new layout attributes object configured with the initial attributes for the inter-item gap view.

## Discussion

Call this method when you need to create a layout attributes object for an inter-item gap view in a collection view. Gap views are used during drag and drop to indicate the area where content will drop. This method uses the parameters to set the initial values of the indexPath property of the returned object. The representedElementKind property is set to elementKindInterItemGapIndicator.

## See Also

### Creating Layout Attributes

convenience init(forItemWith: IndexPath)

Creates and returns a layout attributes object for the item at the specified index path.

convenience init(forSupplementaryViewOfKind: NSCollectionView.SupplementaryElementKind, with: IndexPath)

Creates and returns a layout attributes object for a supplementary view based on the specified information.

convenience init(forDecorationViewOfKind: NSCollectionView.DecorationElementKind, with: IndexPath)

Creates and returns a layout attributes object for a decoration view based on the specified information.

typealias DecorationElementKind

