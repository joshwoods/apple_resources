

- UIKit
- UIPointerRegion
-  identifier 

Instance Property

# identifier

An optional identifier for the region.

iOS 13.4+iPadOS 13.4+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
var identifier: AnyHashable? { get }
```

## Discussion

Use this value to identify the UIPointerRegion in subsequent pointer interaction delegate calls.

## See Also

### Configuring a region

var rect: CGRect

The rectangle bounds of the region.

var latchingAxes: UIAxis

Axes along which the region latches after a primary click.

