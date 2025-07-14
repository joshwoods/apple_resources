

- UIKit
- UICollectionViewFlowLayoutInvalidationContext
-  invalidateFlowLayoutDelegateMetrics 

Instance Property

# invalidateFlowLayoutDelegateMetrics

A Boolean indicating whether to recompute the size of items and views in the layout.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var invalidateFlowLayoutDelegateMetrics: Bool { get set }
```

## Discussion

The default value of this property is false. Set this property to true if you’re invalidating the layout because of changes to the size of any items.

When this property is set to true, the flow layout object recomputes the size of its items and views, querying the delegate object as needed for that information.

## See Also

### Specifying what to invalidate

var invalidateFlowLayoutAttributes: Bool

A Boolean indicating whether to recompute the layout attributes for items and views in the layout.

