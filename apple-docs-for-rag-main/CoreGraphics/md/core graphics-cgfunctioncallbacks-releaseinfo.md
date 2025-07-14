

- Core Graphics
- CGFunctionCallbacks
-  releaseInfo 

Instance Property

# releaseInfo

If non-`NULL`,the callback used to release the `info` parameterpassed to init(info:domainDimension:domain:rangeDimension:range:callbacks:).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var releaseInfo: CGFunctionReleaseInfoCallback?
```

## See Also

### Instance Properties

var evaluate: CGFunctionEvaluateCallback?

The callback that evaluates the function.

var version: UInt32

The structure version number. For this structure,the version should be `0`.

