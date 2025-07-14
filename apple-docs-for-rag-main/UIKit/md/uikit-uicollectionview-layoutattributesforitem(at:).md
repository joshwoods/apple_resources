

- UIKit
- UICollectionView
-  layoutAttributesForItem(at:) 

Instance Method

# layoutAttributesForItem(at:)

Gets the layout information for the item at the specified index path.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func layoutAttributesForItem(at indexPath: IndexPath) -> UICollectionViewLayoutAttributes?
```

## Parameters 

`indexPath`  

The index path of the item.

## Return Value

The layout attributes for the item or `nil` if no item exists at the specified path.

## Discussion

Use this method to retrieve the layout information for a particular item. You should always use this method instead of querying the layout object directly.

## See Also

### Getting layout information

func layoutAttributesForSupplementaryElement(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

Gets the layout information for the specified supplementary view.

