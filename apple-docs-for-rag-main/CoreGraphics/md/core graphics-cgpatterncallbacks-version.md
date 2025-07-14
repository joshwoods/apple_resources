

- Core Graphics
- CGPatternCallbacks
-  version 

Instance Property

# version

The version of the structure passed in as a parameterto the init(info:bounds:matrix:xStep:yStep:tiling:isColored:callbacks:). Forthis version of the structure, you should set this value to zero.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var version: UInt32
```

## See Also

### Instance Properties

var drawPattern: CGPatternDrawPatternCallback?

A pointer to a custom function that draws thepattern. For information about this callback function, see CGPatternDrawPatternCallback.

var releaseInfo: CGPatternReleaseInfoCallback?

An optional pointer to a custom function that’sinvoked when the pattern is released. CGPatternReleaseInfoCallback.

