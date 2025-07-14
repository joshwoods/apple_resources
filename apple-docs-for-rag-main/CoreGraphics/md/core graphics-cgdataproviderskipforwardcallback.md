

- Core Graphics
-  CGDataProviderSkipForwardCallback 

Type Alias

# CGDataProviderSkipForwardCallback

A callback function that advances the current position in the data stream supplied by the provider.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CGDataProviderSkipForwardCallback = (UnsafeMutableRawPointer?, off_t) -> off_t
```

## Parameters 

`info`  

A generic pointer to private data shared among your callback functions. This is the same pointer you supplied to init(version:getBytes:skipForward:rewind:releaseInfo:).

`count`  

The number of bytes to skip.

## Return Value

The number of bytes that were actually skipped.

## Discussion

When Core Graphics needs to advance forward in the provider’s data stream, your function is called.

## See Also

### Creating Sequential-Access Data Providers

init?(sequentialInfo: UnsafeMutableRawPointer?, callbacks: UnsafePointer&lt;CGDataProviderSequentialCallbacks>)

Creates a sequential-access data provider.

struct CGDataProviderSequentialCallbacks

Defines a structure containing pointers to client-defined callback functions that manage the sending of data for a sequential-access data provider.

typealias CGDataProviderRewindCallback

A callback function that moves the current position in the data stream back to the beginning.

typealias CGDataProviderGetBytesCallback

A callback function that copies from a provider data stream into a Core Graphics buffer.

typealias CGDataProviderReleaseInfoCallback

A callback function that releases any private data or resources associated with the data provider.

