

- Core Graphics
- CGDataProviderSequentialCallbacks
-  rewind 

Instance Property

# rewind

A pointer to a function Core Graphics calls to return the provider to the beginning of the data stream. For more information, see CGDataProviderRewindCallback.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var rewind: CGDataProviderRewindCallback?
```

## See Also

### Instance Properties

var getBytes: CGDataProviderGetBytesCallback?

A pointer to a function that copies data from the provider. For more information, see CGDataProviderGetBytesCallback.

var releaseInfo: CGDataProviderReleaseInfoCallback?

A pointer to a function that handles clean-up for the data provider, or `NULL`. For more information, see CGDataProviderReleaseInfoCallback.

var skipForward: CGDataProviderSkipForwardCallback?

A pointer to a function that Core Graphics calls to advance the stream of data supplied by the provider.

var version: UInt32

The version of this structure. It should be set to 0.

