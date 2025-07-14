

- AppKit
- NSCollectionViewLayoutInvalidationContext
-  invalidatedSupplementaryIndexPaths 

Instance Property

# invalidatedSupplementaryIndexPaths

A dictionary containing the supplementary views whose layout attributes are invalid.

macOS 10.11+

``` source
@MainActor
var invalidatedSupplementaryIndexPaths: [NSCollectionView.SupplementaryElementKind : Set]? { get }
```

## Discussion

The keys in this dictionary are the element kind strings of the supplementary views. The value for each key is an NSSet object containing one or more NSIndexPath objects, each of which identifies the section containing the supplementary view.

## See Also

### Invalidating Specific Items

func invalidateItems(at: Set&lt;IndexPath>)

Marks the specified items as invalid so that their layout information can be updated.

func invalidateSupplementaryElements(ofKind: NSCollectionView.SupplementaryElementKind, at: Set&lt;IndexPath>)

Marks the specified supplementary views as invalid so that their layout information can be updated.

func invalidateDecorationElements(ofKind: NSCollectionView.DecorationElementKind, at: Set&lt;IndexPath>)

Marks the specified decoration views as invalid so that their layout information can be updated.

var invalidatedItemIndexPaths: Set&lt;IndexPath>?

The set of items whose layout attributes are invalid.

var invalidatedDecorationIndexPaths: [NSCollectionView.DecorationElementKind : Set&lt;IndexPath>]?

A dictionary containing the decoration views whose layout attributes are invalid.

