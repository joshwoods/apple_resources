

- AppKit
- NSCollectionViewLayoutInvalidationContext
-  invalidatedItemIndexPaths 

Instance Property

# invalidatedItemIndexPaths

The set of items whose layout attributes are invalid.

macOS 10.11+

``` source
@MainActor
var invalidatedItemIndexPaths: Set? { get }
```

## Discussion

The set contains zero or more NSIndexPath objects, each of which identifies an invalid item.

## See Also

### Invalidating Specific Items

func invalidateItems(at: Set&lt;IndexPath>)

Marks the specified items as invalid so that their layout information can be updated.

func invalidateSupplementaryElements(ofKind: NSCollectionView.SupplementaryElementKind, at: Set&lt;IndexPath>)

Marks the specified supplementary views as invalid so that their layout information can be updated.

func invalidateDecorationElements(ofKind: NSCollectionView.DecorationElementKind, at: Set&lt;IndexPath>)

Marks the specified decoration views as invalid so that their layout information can be updated.

var invalidatedSupplementaryIndexPaths: [NSCollectionView.SupplementaryElementKind : Set&lt;IndexPath>]?

A dictionary containing the supplementary views whose layout attributes are invalid.

var invalidatedDecorationIndexPaths: [NSCollectionView.DecorationElementKind : Set&lt;IndexPath>]?

A dictionary containing the decoration views whose layout attributes are invalid.

