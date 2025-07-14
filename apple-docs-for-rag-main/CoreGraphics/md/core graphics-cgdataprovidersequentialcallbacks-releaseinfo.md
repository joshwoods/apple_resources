

- Core Graphics
- CGDataProviderSequentialCallbacks
-  releaseInfo 

Instance Property

# releaseInfo

A pointer to a function that handles clean-up for the data provider, or `NULL`. For more information, see CGDataProviderReleaseInfoCallback.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var releaseInfo: CGDataProviderReleaseInfoCallback?
```

## See Also

### Instance Properties

var getBytes: CGDataProviderGetBytesCallback?

A pointer to a function that copies data from the provider. For more information, see CGDataProviderGetBytesCallback.

var rewind: CGDataProviderRewindCallback?

A pointer to a function Core Graphics calls to return the provider to the beginning of the data stream. For more information, see CGDataProviderRewindCallback.

var skipForward: CGDataProviderSkipForwardCallback?

A pointer to a function that Core Graphics calls to advance the stream of data supplied by the provider.

var version: UInt32

The version of this structure. It should be set to 0.

