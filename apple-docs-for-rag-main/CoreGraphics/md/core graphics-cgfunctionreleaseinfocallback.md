

- Core Graphics
-  CGFunctionReleaseInfoCallback 

Type Alias

# CGFunctionReleaseInfoCallback

Performs custom clean-up tasks when Core Graphics deallocates a `CGFunctionRef` object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CGFunctionReleaseInfoCallback = (UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`info`  

The `info` parameter passed to init(info:domainDimension:domain:rangeDimension:range:callbacks:).

## See Also

### Callbacks

struct CGFunctionCallbacks

A structure that contains callbacks needed by a `CGFunctionRef` object.

typealias CGFunctionEvaluateCallback

Performs custom operations on the supplied input data to produce output data.

