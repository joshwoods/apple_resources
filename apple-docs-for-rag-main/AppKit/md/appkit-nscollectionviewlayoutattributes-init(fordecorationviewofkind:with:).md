

- AppKit
- NSCollectionViewLayoutAttributes
-  init(forDecorationViewOfKind:with:) 

Initializer

# init(forDecorationViewOfKind:with:)

Creates and returns a layout attributes object for a decoration view based on the specified information.

macOS 10.11+

``` source
@MainActor
convenience init(
    forDecorationViewOfKind decorationViewKind: NSCollectionView.DecorationElementKind,
    with indexPath: IndexPath
)
```

## Parameters 

`decorationViewKind`  

A string that identifies the type of the decoration view. Use this string to differentiate from among the decoration views in a given section. This parameter must contain a valid value.

`indexPath`  

The index path of the item. You can use this information to identify the item in your app’s data structures.

## Return Value

A new layout attributes object configured with the initial attributes for the decoration view.

## Discussion

Call this method when you need to create a layout attributes object for a decoration view in a collection view. Decoration views are a tertiary type of content that display visual adornments in your collection view interface. For example, decoration views might display custom backgrounds. This method uses the parameters to set the initial values of the indexPath and representedElementKind properties the returned object.

## See Also

### Creating Layout Attributes

convenience init(forItemWith: IndexPath)

Creates and returns a layout attributes object for the item at the specified index path.

convenience init(forSupplementaryViewOfKind: NSCollectionView.SupplementaryElementKind, with: IndexPath)

Creates and returns a layout attributes object for a supplementary view based on the specified information.

convenience init(forInterItemGapBefore: IndexPath)

Creates and returns a layout attributes object for an inter-item gap view at the specified index path.

typealias DecorationElementKind

