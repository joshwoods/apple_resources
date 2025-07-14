

- Core Graphics
- CGDataProviderDirectCallbacks
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

var getBytePointer: CGDataProviderGetBytePointerCallback?

A pointer to a function that returns a pointer to the provider’s data. For more information, see CGDataProviderGetBytePointerCallback.

var getBytesAtPosition: CGDataProviderGetBytesAtPositionCallback?

A pointer to a function that copies data from the provider.

var releaseBytePointer: CGDataProviderReleaseBytePointerCallback?

A pointer to a function that Core Graphics calls to release a pointer to the provider’s data. For more information, see CGDataProviderReleaseBytePointerCallback.

var releaseInfo: CGDataProviderReleaseInfoCallback?

A pointer to a function that handles clean-up for the data provider, or `NULL`. For more information, see CGDataProviderReleaseInfoCallback.

