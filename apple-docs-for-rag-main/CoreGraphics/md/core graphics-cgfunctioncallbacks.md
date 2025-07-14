

- Core Graphics
-  CGFunctionCallbacks 

Structure

# CGFunctionCallbacks

A structure that contains callbacks needed by a `CGFunctionRef` object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CGFunctionCallbacks
```

## Topics

### Initializers

init()

init(version: UInt32, evaluate: CGFunctionEvaluateCallback?, releaseInfo: CGFunctionReleaseInfoCallback?)

### Instance Properties

var evaluate: CGFunctionEvaluateCallback?

The callback that evaluates the function.

var releaseInfo: CGFunctionReleaseInfoCallback?

If non-`NULL`,the callback used to release the `info` parameterpassed to init(info:domainDimension:domain:rangeDimension:range:callbacks:).

var version: UInt32

The structure version number. For this structure,the version should be `0`.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Callbacks

typealias CGFunctionEvaluateCallback

Performs custom operations on the supplied input data to produce output data.

typealias CGFunctionReleaseInfoCallback

Performs custom clean-up tasks when Core Graphics deallocates a `CGFunctionRef` object.

