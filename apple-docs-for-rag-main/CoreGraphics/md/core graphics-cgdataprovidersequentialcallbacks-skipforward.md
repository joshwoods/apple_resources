

- Core Graphics
- CGDataProviderSequentialCallbacks
-  skipForward 

Instance Property

# skipForward

A pointer to a function that Core Graphics calls to advance the stream of data supplied by the provider.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var skipForward: CGDataProviderSkipForwardCallback?
```

## See Also

### Instance Properties

var getBytes: CGDataProviderGetBytesCallback?

A pointer to a function that copies data from the provider. For more information, see CGDataProviderGetBytesCallback.

var releaseInfo: CGDataProviderReleaseInfoCallback?

A pointer to a function that handles clean-up for the data provider, or `NULL`. For more information, see CGDataProviderReleaseInfoCallback.

var rewind: CGDataProviderRewindCallback?

A pointer to a function Core Graphics calls to return the provider to the beginning of the data stream. For more information, see CGDataProviderRewindCallback.

var version: UInt32

The version of this structure. It should be set to 0.

