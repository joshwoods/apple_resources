

- Core Graphics
- CGDataProviderSequentialCallbacks
-  version 

Instance Property

# version

The version of this structure. It should be set to 0.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var version: UInt32
```

## See Also

### Instance Properties

var getBytes: CGDataProviderGetBytesCallback?

A pointer to a function that copies data from the provider. For more information, see CGDataProviderGetBytesCallback.

var releaseInfo: CGDataProviderReleaseInfoCallback?

A pointer to a function that handles clean-up for the data provider, or `NULL`. For more information, see CGDataProviderReleaseInfoCallback.

var rewind: CGDataProviderRewindCallback?

A pointer to a function Core Graphics calls to return the provider to the beginning of the data stream. For more information, see CGDataProviderRewindCallback.

var skipForward: CGDataProviderSkipForwardCallback?

A pointer to a function that Core Graphics calls to advance the stream of data supplied by the provider.

