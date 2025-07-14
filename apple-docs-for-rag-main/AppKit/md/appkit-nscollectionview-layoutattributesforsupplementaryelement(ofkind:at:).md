

- AppKit
- NSCollectionView
-  layoutAttributesForSupplementaryElement(ofKind:at:) 

Instance Method

# layoutAttributesForSupplementaryElement(ofKind:at:)

Returns the layout information for the supplementary view at the specified index path.

macOS 10.11+

``` source
@MainActor
func layoutAttributesForSupplementaryElement(
    ofKind kind: NSCollectionView.SupplementaryElementKind,
    at indexPath: IndexPath
) -> NSCollectionViewLayoutAttributes?
```

## Parameters 

`kind`  

The kind of the supplementary view whose attributes you want. The layout object defines the kinds of supplementary views it supports. This parameter must not be `nil`.

`indexPath`  

The index path of the supplementary view. Normally, this path

## Return Value

The layout attributes of the supplementary view or `nil` if no item exists at the specified path.

## Discussion

This method updates the layout information as needed before returning the specified attributes. Always use this method to retrieve the layout attributes for supplementary views in the collection view. Do not query the layout object directly.

## See Also

### Getting Layout Information

func layoutAttributesForItem(at: IndexPath) -> NSCollectionViewLayoutAttributes?

Returns the layout information for the item at the specified index path.

