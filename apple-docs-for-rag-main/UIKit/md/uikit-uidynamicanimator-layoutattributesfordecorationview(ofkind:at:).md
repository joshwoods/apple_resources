

- UIKit
- UIDynamicAnimator
-  layoutAttributesForDecorationView(ofKind:at:) 

Instance Method

# layoutAttributesForDecorationView(ofKind:at:)

A convenience method for returning the layout attributes for a collection view decoration view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
func layoutAttributesForDecorationView(
    ofKind decorationViewKind: String,
    at indexPath: IndexPath
) -> UICollectionViewLayoutAttributes?
```

## Parameters 

`decorationViewKind`  

The kind identifier for the specified decoration view.

`indexPath`  

The index path for the cell whose decoration view layout attributes you want.

## Return Value

The collection view layout attributes for the specified decoration view.

## See Also

### Working with collection views

func layoutAttributesForCell(at: IndexPath) -> UICollectionViewLayoutAttributes?

A convenience method for returning the layout attributes for a collection view cell.

func layoutAttributesForSupplementaryView(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

A convenience method for returning the layout attributes for a collection view supplementary view.

