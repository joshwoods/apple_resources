

- Core Graphics
-  CGDataProviderReleaseBytePointerCallback 

Type Alias

# CGDataProviderReleaseBytePointerCallback

A callback function that releases the pointer Core Graphics obtained by calling CGDataProviderGetBytePointerCallback.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CGDataProviderReleaseBytePointerCallback = (UnsafeMutableRawPointer?, UnsafeRawPointer) -> Void
```

## Parameters 

`info`  

A generic pointer to private data shared among your callback functions. This is the same pointer you supplied to `CGDataProviderCreateDirectAccess`.

`pointer`  

A pointer to your provider data. This is the same pointer you returned in CGDataProviderGetBytePointerCallback.

## Discussion

When Core Graphics no longer needs direct access to your provider data, your function is called. You may safely modify, move, or release your provider data at this time.

For information on how to associate your function with a direct-access data provider, see `CGDataProviderCreateDirectAccess` and `CGDataProviderDirectAccessCallbacks`.

## See Also

### Creating Direct-Access Data Providers

init?(directInfo: UnsafeMutableRawPointer?, size: off_t, callbacks: UnsafePointer&lt;CGDataProviderDirectCallbacks>)

Creates a direct-access data provider.

init?(data: CFData)

Creates a data provider that reads from a CFData object.

init?(url: CFURL)

Creates a direct-access data provider that uses a URL to supply data.

init?(dataInfo: UnsafeMutableRawPointer?, data: UnsafeRawPointer, size: Int, releaseData: CGDataProviderReleaseDataCallback)

Creates a direct-access data provider that uses data your program supplies.

init?(filename: UnsafePointer&lt;CChar>)

Creates a direct-access data provider that uses a file to supply data.

struct CGDataProviderDirectCallbacks

Defines pointers to client-defined callback functions that manage the sending of data for a direct-access data provider.

typealias CGDataProviderGetBytePointerCallback

A callback function that returns a generic pointer to the provider data.

typealias CGDataProviderGetBytesAtPositionCallback

A callback function that copies data from the provider into a Core Graphics buffer.

typealias CGDataProviderReleaseInfoCallback

A callback function that releases any private data or resources associated with the data provider.

typealias CGDataProviderReleaseDataCallback

A callback function that releases data you supply to the function init(dataInfo:data:size:releaseData:).

