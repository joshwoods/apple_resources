

- UIKit
- UIDynamicAnimator
-  layoutAttributesForSupplementaryView(ofKind:at:) 

Instance Method

# layoutAttributesForSupplementaryView(ofKind:at:)

A convenience method for returning the layout attributes for a collection view supplementary view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
func layoutAttributesForSupplementaryView(
    ofKind kind: String,
    at indexPath: IndexPath
) -> UICollectionViewLayoutAttributes?
```

## Parameters 

`kind`  

A string that identifies the type of supplementary view whose layout attributes you want.

`indexPath`  

The index path for the cell whose supplementary view layout attributes you want.

## Return Value

The collection view layout attributes for the specified supplementary view.

## See Also

### Working with collection views

func layoutAttributesForCell(at: IndexPath) -> UICollectionViewLayoutAttributes?

A convenience method for returning the layout attributes for a collection view cell.

func layoutAttributesForDecorationView(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

A convenience method for returning the layout attributes for a collection view decoration view.

