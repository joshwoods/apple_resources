

- Core Graphics
-  CGDataProviderRewindCallback 

Type Alias

# CGDataProviderRewindCallback

A callback function that moves the current position in the data stream back to the beginning.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CGDataProviderRewindCallback = (UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`info`  

A generic pointer to private data shared among your callback functions. This is the same pointer you supplied to init(version:getBytes:skipForward:rewind:releaseInfo:).

## Discussion

When Core Graphics needs to read from the beginning of the provider’s data stream, your function is called.

For information on how to associate your callback function with a data provider, see CGDataProvider and CGDataProviderSequentialCallbacks.

## See Also

### Creating Sequential-Access Data Providers

init?(sequentialInfo: UnsafeMutableRawPointer?, callbacks: UnsafePointer&lt;CGDataProviderSequentialCallbacks>)

Creates a sequential-access data provider.

struct CGDataProviderSequentialCallbacks

Defines a structure containing pointers to client-defined callback functions that manage the sending of data for a sequential-access data provider.

typealias CGDataProviderGetBytesCallback

A callback function that copies from a provider data stream into a Core Graphics buffer.

typealias CGDataProviderSkipForwardCallback

A callback function that advances the current position in the data stream supplied by the provider.

typealias CGDataProviderReleaseInfoCallback

A callback function that releases any private data or resources associated with the data provider.

