

- UIKit
- UICollectionViewLayoutInvalidationContext
-  invalidateDecorationElements(ofKind:at:) 

Instance Method

# invalidateDecorationElements(ofKind:at:)

Adds the decoration views at the specified index paths to the list of invalid items.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func invalidateDecorationElements(
    ofKind elementKind: String,
    at indexPaths: [IndexPath]
)
```

## Parameters 

`elementKind`  

A string that identifies the type of the decoration views. This parameter must not be `nil`.

`indexPaths`  

An array of NSIndexPath objects. Each index path represents a supplementary view of the given kind whose layout needs to be recomputed.

## Discussion

Call this method to identify the specific decoration views whose layout attributes changed. The views you specify are added to the dictionary in the invalidatedDecorationIndexPaths property. All of the views you specify should be of the type that you specified in the `elementKind` parameter. If you call this method two or more times with the same value for the `elementKind` parameter, this method merges the new index paths with the ones previously specified.

## See Also

### Invalidating Specific Items

func invalidateItems(at: [IndexPath])

Adds the cells at the specified index paths to the list of invalid items.

func invalidateSupplementaryElements(ofKind: String, at: [IndexPath])

Adds the supplementary views at the specified index paths to the list of invalid items.

var invalidatedItemIndexPaths: [IndexPath]?

An array of index paths representing the cells that were invalidated.

var invalidatedSupplementaryIndexPaths: [String : [IndexPath]]?

A dictionary that identifies the supplementary views that were invalidated.

var invalidatedDecorationIndexPaths: [String : [IndexPath]]?

A dictionary that identifies the decoration views that were invalidated.

