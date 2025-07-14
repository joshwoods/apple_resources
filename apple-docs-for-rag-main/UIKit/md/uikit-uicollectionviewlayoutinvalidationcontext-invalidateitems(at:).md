

- UIKit
- UICollectionViewLayoutInvalidationContext
-  invalidateItems(at:) 

Instance Method

# invalidateItems(at:)

Adds the cells at the specified index paths to the list of invalid items.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func invalidateItems(at indexPaths: [IndexPath])
```

## Parameters 

`indexPaths`  

An array of NSIndexPath objects. Each index path represents a cell whose layout needs to be recomputed.

## Discussion

Call this method to identify the specific cells of your layout that require updates. The cells you specify are added to the array in the invalidatedItemIndexPaths property.

## See Also

### Invalidating Specific Items

func invalidateSupplementaryElements(ofKind: String, at: [IndexPath])

Adds the supplementary views at the specified index paths to the list of invalid items.

func invalidateDecorationElements(ofKind: String, at: [IndexPath])

Adds the decoration views at the specified index paths to the list of invalid items.

var invalidatedItemIndexPaths: [IndexPath]?

An array of index paths representing the cells that were invalidated.

var invalidatedSupplementaryIndexPaths: [String : [IndexPath]]?

A dictionary that identifies the supplementary views that were invalidated.

var invalidatedDecorationIndexPaths: [String : [IndexPath]]?

A dictionary that identifies the decoration views that were invalidated.

