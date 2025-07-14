

- Core Graphics
- CGPatternCallbacks
-  releaseInfo 

Instance Property

# releaseInfo

An optional pointer to a custom function that’sinvoked when the pattern is released. CGPatternReleaseInfoCallback.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var releaseInfo: CGPatternReleaseInfoCallback?
```

## See Also

### Instance Properties

var drawPattern: CGPatternDrawPatternCallback?

A pointer to a custom function that draws thepattern. For information about this callback function, see CGPatternDrawPatternCallback.

var version: UInt32

The version of the structure passed in as a parameterto the init(info:bounds:matrix:xStep:yStep:tiling:isColored:callbacks:). Forthis version of the structure, you should set this value to zero.

