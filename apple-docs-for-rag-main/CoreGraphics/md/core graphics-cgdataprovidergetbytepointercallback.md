

- Core Graphics
-  CGDataProviderGetBytePointerCallback 

Type Alias

# CGDataProviderGetBytePointerCallback

A callback function that returns a generic pointer to the provider data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CGDataProviderGetBytePointerCallback = (UnsafeMutableRawPointer?) -> UnsafeRawPointer?
```

## Parameters 

`info`  

A generic pointer to private data shared among your callback functions. This is the same pointer you supplied to `CGDataProviderCreateDirectAccess`.

## Return Value

A generic pointer to your provider data. By suppling this pointer, you are giving Core Graphics read-only access to both the pointer and the underlying provider data. You must not move or modify the provider data until Core Graphics calls your CGDataProviderReleaseBytePointerCallback function.

## Discussion

When Core Graphics needs direct access to your provider data, this function is called.

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

typealias CGDataProviderGetBytesAtPositionCallback

A callback function that copies data from the provider into a Core Graphics buffer.

typealias CGDataProviderReleaseBytePointerCallback

A callback function that releases the pointer Core Graphics obtained by calling CGDataProviderGetBytePointerCallback.

typealias CGDataProviderReleaseInfoCallback

A callback function that releases any private data or resources associated with the data provider.

typealias CGDataProviderReleaseDataCallback

A callback function that releases data you supply to the function init(dataInfo:data:size:releaseData:).

