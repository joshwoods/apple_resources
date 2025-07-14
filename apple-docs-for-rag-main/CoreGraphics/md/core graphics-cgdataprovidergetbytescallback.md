

- Core Graphics
-  CGDataProviderGetBytesCallback 

Type Alias

# CGDataProviderGetBytesCallback

A callback function that copies from a provider data stream into a Core Graphics buffer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CGDataProviderGetBytesCallback = (UnsafeMutableRawPointer?, UnsafeMutableRawPointer, Int) -> Int
```

## Parameters 

`info`  

A generic pointer to private data shared among your callback functions. This is the same pointer you supplied to init(version:getBytes:skipForward:rewind:releaseInfo:).

`buffer`  

The Core Graphics buffer into which you copy the specified number of bytes.

`count`  

The number of bytes to copy.

## Return Value

The number of bytes copied. If no more data can be written to the buffer, you should return `0`.

## Discussion

When Core Graphics is ready to receive data from the provider data stream, your function is called. It should copy the specified number of bytes into `buffer`.

For information on how to associate your callback function with a data provider, see CGDataProvider and CGDataProviderSequentialCallbacks.

## See Also

### Creating Sequential-Access Data Providers

init?(sequentialInfo: UnsafeMutableRawPointer?, callbacks: UnsafePointer&lt;CGDataProviderSequentialCallbacks>)

Creates a sequential-access data provider.

struct CGDataProviderSequentialCallbacks

Defines a structure containing pointers to client-defined callback functions that manage the sending of data for a sequential-access data provider.

typealias CGDataProviderRewindCallback

A callback function that moves the current position in the data stream back to the beginning.

typealias CGDataProviderSkipForwardCallback

A callback function that advances the current position in the data stream supplied by the provider.

typealias CGDataProviderReleaseInfoCallback

A callback function that releases any private data or resources associated with the data provider.

