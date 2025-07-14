

- AppKit
- NSCollectionViewLayoutInvalidationContext
-  invalidateItems(at:) 

Instance Method

# invalidateItems(at:)

Marks the specified items as invalid so that their layout information can be updated.

macOS 10.11+

``` source
@MainActor
func invalidateItems(at indexPaths: Set)
```

## Parameters 

`indexPaths`  

A set of NSIndexPath objects. Each index path represents an item whose layout needs to be recomputed.

## Discussion

Call this method when you want the layout object to recompute attributes for a specific set of items. The items you provide are added to the invalidatedItemIndexPaths property. You can call this method more than once to create a merged set of items.

## See Also

### Invalidating Specific Items

func invalidateSupplementaryElements(ofKind: NSCollectionView.SupplementaryElementKind, at: Set&lt;IndexPath>)

Marks the specified supplementary views as invalid so that their layout information can be updated.

func invalidateDecorationElements(ofKind: NSCollectionView.DecorationElementKind, at: Set&lt;IndexPath>)

Marks the specified decoration views as invalid so that their layout information can be updated.

var invalidatedItemIndexPaths: Set&lt;IndexPath>?

The set of items whose layout attributes are invalid.

var invalidatedSupplementaryIndexPaths: [NSCollectionView.SupplementaryElementKind : Set&lt;IndexPath>]?

A dictionary containing the supplementary views whose layout attributes are invalid.

var invalidatedDecorationIndexPaths: [NSCollectionView.DecorationElementKind : Set&lt;IndexPath>]?

A dictionary containing the decoration views whose layout attributes are invalid.

