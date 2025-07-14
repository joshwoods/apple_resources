

- UIKit
- UICollectionViewFlowLayoutInvalidationContext
-  invalidateFlowLayoutAttributes 

Instance Property

# invalidateFlowLayoutAttributes

A Boolean indicating whether to recompute the layout attributes for items and views in the layout.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var invalidateFlowLayoutAttributes: Bool { get set }
```

## Discussion

The default value of this property is false. Set this property to true if there are changes to the position of items on the screen. For example, the flow layout object sets this property to true when the collection view’s bounds change in a way that affects the number of items in a column or row.

When this property is set to true, the flow layout object recomputes the layout attributes for its items and views. If the invalidateFlowLayoutDelegateMetrics property is set to false it recomputes this information without asking for new size information.

## See Also

### Specifying what to invalidate

var invalidateFlowLayoutDelegateMetrics: Bool

A Boolean indicating whether to recompute the size of items and views in the layout.

