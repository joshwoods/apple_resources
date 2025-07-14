

- UIKit
- UIPointerRegion
-  latchingAxes 

Instance Property

# latchingAxes

Axes along which the region latches after a primary click.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
var latchingAxes: UIAxis { get set }
```

## Discussion

If you set this property, the UIPointerStyle associated with this region locks in and only allows freeform movement along the axes you specify.

## See Also

### Configuring a region

var rect: CGRect

The rectangle bounds of the region.

var identifier: AnyHashable?

An optional identifier for the region.

