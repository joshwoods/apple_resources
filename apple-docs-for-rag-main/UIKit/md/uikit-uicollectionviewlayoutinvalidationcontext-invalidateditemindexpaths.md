

- UIKit
- UICollectionViewLayoutInvalidationContext
-  invalidatedItemIndexPaths 

Instance Property

# invalidatedItemIndexPaths

An array of index paths representing the cells that were invalidated.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var invalidatedItemIndexPaths: [IndexPath]? { get }
```

## Discussion

The array contains zero or more NSIndexPath objects, each of which represents a cell whose layout changed.

## See Also

### Invalidating Specific Items

func invalidateItems(at: [IndexPath])

Adds the cells at the specified index paths to the list of invalid items.

func invalidateSupplementaryElements(ofKind: String, at: [IndexPath])

Adds the supplementary views at the specified index paths to the list of invalid items.

func invalidateDecorationElements(ofKind: String, at: [IndexPath])

Adds the decoration views at the specified index paths to the list of invalid items.

var invalidatedSupplementaryIndexPaths: [String : [IndexPath]]?

A dictionary that identifies the supplementary views that were invalidated.

var invalidatedDecorationIndexPaths: [String : [IndexPath]]?

A dictionary that identifies the decoration views that were invalidated.

