

- Core Graphics
- CGFunctionCallbacks
-  version 

Instance Property

# version

The structure version number. For this structure,the version should be `0`.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var version: UInt32
```

## See Also

### Instance Properties

var evaluate: CGFunctionEvaluateCallback?

The callback that evaluates the function.

var releaseInfo: CGFunctionReleaseInfoCallback?

If non-`NULL`,the callback used to release the `info` parameterpassed to init(info:domainDimension:domain:rangeDimension:range:callbacks:).

