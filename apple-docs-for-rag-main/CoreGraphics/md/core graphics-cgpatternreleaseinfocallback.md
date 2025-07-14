

- Core Graphics
-  CGPatternReleaseInfoCallback 

Type Alias

# CGPatternReleaseInfoCallback

Release private data or resources associated with the pattern.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CGPatternReleaseInfoCallback = (UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`info`  

A generic pointer to private data shared among your callback functions. This is the same pointer you supplied to init(info:bounds:matrix:xStep:yStep:tiling:isColored:callbacks:).

## Discussion

Quartz calls your release function when it frees your pattern object.

To learn how to associate your release function with a Quartz pattern, see init(info:bounds:matrix:xStep:yStep:tiling:isColored:callbacks:) and CGPatternCallbacks.

## See Also

### Callbacks

struct CGPatternCallbacks

A structure that holds a version and two callback functions for drawing a custom pattern.

typealias CGPatternDrawPatternCallback

Draws a pattern cell.

