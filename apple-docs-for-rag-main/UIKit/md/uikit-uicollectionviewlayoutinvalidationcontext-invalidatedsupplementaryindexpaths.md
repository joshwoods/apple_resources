

- UIKit
- UICollectionViewLayoutInvalidationContext
-  invalidatedSupplementaryIndexPaths 

Instance Property

# invalidatedSupplementaryIndexPaths

A dictionary that identifies the supplementary views that were invalidated.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var invalidatedSupplementaryIndexPaths: [String : [IndexPath]]? { get }
```

## Discussion

The keys in this dictionary are the element kind strings of the invalid supplementary views. The value for each key is an array of NSIndexPath objects indicating which specific supplementary views have layout changes.

## See Also

### Invalidating Specific Items

func invalidateItems(at: [IndexPath])

Adds the cells at the specified index paths to the list of invalid items.

func invalidateSupplementaryElements(ofKind: String, at: [IndexPath])

Adds the supplementary views at the specified index paths to the list of invalid items.

func invalidateDecorationElements(ofKind: String, at: [IndexPath])

Adds the decoration views at the specified index paths to the list of invalid items.

var invalidatedItemIndexPaths: [IndexPath]?

An array of index paths representing the cells that were invalidated.

var invalidatedDecorationIndexPaths: [String : [IndexPath]]?

A dictionary that identifies the decoration views that were invalidated.

