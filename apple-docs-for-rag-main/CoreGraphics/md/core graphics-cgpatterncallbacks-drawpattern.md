

- Core Graphics
- CGPatternCallbacks
-  drawPattern 

Instance Property

# drawPattern

A pointer to a custom function that draws thepattern. For information about this callback function, see CGPatternDrawPatternCallback.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var drawPattern: CGPatternDrawPatternCallback?
```

## See Also

### Instance Properties

var releaseInfo: CGPatternReleaseInfoCallback?

An optional pointer to a custom function that’sinvoked when the pattern is released. CGPatternReleaseInfoCallback.

var version: UInt32

The version of the structure passed in as a parameterto the init(info:bounds:matrix:xStep:yStep:tiling:isColored:callbacks:). Forthis version of the structure, you should set this value to zero.

