

- AppKit
- NSCollectionView
-  layoutAttributesForItem(at:) 

Instance Method

# layoutAttributesForItem(at:)

Returns the layout information for the item at the specified index path.

macOS 10.11+

``` source
@MainActor
func layoutAttributesForItem(at indexPath: IndexPath) -> NSCollectionViewLayoutAttributes?
```

## Parameters 

`indexPath`  

The index path of the item.

## Return Value

The layout attributes of the item or `nil` if no item exists at the specified path.

## Discussion

This method updates the layout information as needed before returning the specified attributes. Always use this method to retrieve the layout attributes for items in the collection view. Do not query the layout object directly.

## See Also

### Getting Layout Information

func layoutAttributesForSupplementaryElement(ofKind: NSCollectionView.SupplementaryElementKind, at: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns the layout information for the supplementary view at the specified index path.

