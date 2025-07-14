

- Core Graphics
- CGDataProviderDirectCallbacks
-  releaseBytePointer 

Instance Property

# releaseBytePointer

A pointer to a function that Core Graphics calls to release a pointer to the provider’s data. For more information, see CGDataProviderReleaseBytePointerCallback.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var releaseBytePointer: CGDataProviderReleaseBytePointerCallback?
```

## See Also

### Instance Properties

var getBytePointer: CGDataProviderGetBytePointerCallback?

A pointer to a function that returns a pointer to the provider’s data. For more information, see CGDataProviderGetBytePointerCallback.

var getBytesAtPosition: CGDataProviderGetBytesAtPositionCallback?

A pointer to a function that copies data from the provider.

var releaseInfo: CGDataProviderReleaseInfoCallback?

A pointer to a function that handles clean-up for the data provider, or `NULL`. For more information, see CGDataProviderReleaseInfoCallback.

var version: UInt32

The version of this structure. It should be set to 0.

