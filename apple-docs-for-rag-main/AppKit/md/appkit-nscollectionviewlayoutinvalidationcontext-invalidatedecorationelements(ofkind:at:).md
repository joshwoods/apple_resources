

- AppKit
- NSCollectionViewLayoutInvalidationContext
-  invalidateDecorationElements(ofKind:at:) 

Instance Method

# invalidateDecorationElements(ofKind:at:)

Marks the specified decoration views as invalid so that their layout information can be updated.

macOS 10.11+

``` source
@MainActor
func invalidateDecorationElements(
    ofKind elementKind: NSCollectionView.DecorationElementKind,
    at indexPaths: Set
)
```

## Parameters 

`elementKind`  

A string that identifies the type of the decoration views. This parameter must not be `nil` or an empty string.

`indexPaths`  

A set of NSIndexPath objects. Each index path contains the section in which the decoration view appears.

## Discussion

Call this method when you want the layout object to recompute attributes for one or more decoration views. All of the views must be of the type specified by the `elementKind` parameter. The method adds the views you specify to the invalidatedDecorationIndexPaths property. You can call this method more than once for the specified `elementKind` value.

## See Also

### Invalidating Specific Items

func invalidateItems(at: Set&lt;IndexPath>)

Marks the specified items as invalid so that their layout information can be updated.

func invalidateSupplementaryElements(ofKind: NSCollectionView.SupplementaryElementKind, at: Set&lt;IndexPath>)

Marks the specified supplementary views as invalid so that their layout information can be updated.

var invalidatedItemIndexPaths: Set&lt;IndexPath>?

The set of items whose layout attributes are invalid.

var invalidatedSupplementaryIndexPaths: [NSCollectionView.SupplementaryElementKind : Set&lt;IndexPath>]?

A dictionary containing the supplementary views whose layout attributes are invalid.

var invalidatedDecorationIndexPaths: [NSCollectionView.DecorationElementKind : Set&lt;IndexPath>]?

A dictionary containing the decoration views whose layout attributes are invalid.

