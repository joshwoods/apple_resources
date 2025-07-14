

- AppKit
- NSCollectionViewFlowLayoutInvalidationContext
-  invalidateFlowLayoutAttributes 

Instance Property

# invalidateFlowLayoutAttributes

A Boolean value indicating whether the flow layout object should invalidate its current attributes.

macOS 10.11+

``` source
@MainActor
var invalidateFlowLayoutAttributes: Bool { get set }
```

## Discussion

Setting this property to false tells the flow layout object to keep its existing layout information, effectively stopping the invalidation process. Typically, you set this property to false only if you subclass NSCollectionViewFlowLayout and update changed layout information directly.

The default value of this property is true, which causes the flow layout object to throw out its existing layout information and recompute it.

## See Also

### Invalidating the Flow Layout

var invalidateFlowLayoutDelegateMetrics: Bool

A Boolean value indicating whether the flow layout object should fetch new size information from its delegate.

