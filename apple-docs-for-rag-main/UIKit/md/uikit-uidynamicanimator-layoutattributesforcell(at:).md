

- UIKit
- UIDynamicAnimator
-  layoutAttributesForCell(at:) 

Instance Method

# layoutAttributesForCell(at:)

A convenience method for returning the layout attributes for a collection view cell.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
func layoutAttributesForCell(at indexPath: IndexPath) -> UICollectionViewLayoutAttributes?
```

## Parameters 

`indexPath`  

The index path for the cell whose layout attributes you want.

## Return Value

The collection view layout attributes for the specified collection view cell.

## See Also

### Working with collection views

func layoutAttributesForDecorationView(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

A convenience method for returning the layout attributes for a collection view decoration view.

func layoutAttributesForSupplementaryView(ofKind: String, at: IndexPath) -> UICollectionViewLayoutAttributes?

A convenience method for returning the layout attributes for a collection view supplementary view.

