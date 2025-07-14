

- UIKit
- UIPointerRegion
-  rect 

Instance Property

# rect

The rectangle bounds of the region.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
var rect: CGRect { get }
```

## Discussion

This rectangle must be in the UIPointerInteraction view’s coordinate space.

## See Also

### Configuring a region

var identifier: AnyHashable?

An optional identifier for the region.

var latchingAxes: UIAxis

Axes along which the region latches after a primary click.

