

- AppKit
- NSCollectionViewLayoutAttributes
-  init(forSupplementaryViewOfKind:with:) 

Initializer

# init(forSupplementaryViewOfKind:with:)

Creates and returns a layout attributes object for a supplementary view based on the specified information.

macOS 10.11+

``` source
@MainActor
convenience init(
    forSupplementaryViewOfKind elementKind: NSCollectionView.SupplementaryElementKind,
    with indexPath: IndexPath
)
```

## Parameters 

`elementKind`  

A string that identifies the type of the supplementary view. Use this string to differentiate from among the supplementary views in a given section. This parameter must contain a valid value.

`indexPath`  

The index path of the item. You can use this information to identify the item in your app’s data structures. This parameter must contain a valid value.

## Return Value

A new layout attributes object configured with the initial attributes for the supplementary view.

## Discussion

Call this method when you need to create a layout attributes object for a supplementary view in a collection view. Supplementary views are a secondary type of content that display data related to a specific section. For example, header and footer views in a grid layout implemented using supplementary views. This method uses the parameters to set the initial values of the indexPath and representedElementKind properties the returned object.

## See Also

### Creating Layout Attributes

convenience init(forItemWith: IndexPath)

Creates and returns a layout attributes object for the item at the specified index path.

convenience init(forDecorationViewOfKind: NSCollectionView.DecorationElementKind, with: IndexPath)

Creates and returns a layout attributes object for a decoration view based on the specified information.

convenience init(forInterItemGapBefore: IndexPath)

Creates and returns a layout attributes object for an inter-item gap view at the specified index path.

typealias DecorationElementKind

