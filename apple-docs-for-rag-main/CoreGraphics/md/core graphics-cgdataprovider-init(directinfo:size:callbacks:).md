

- Core Graphics
- CGDataProvider
-  init(directInfo:size:callbacks:) 

Initializer

# init(directInfo:size:callbacks:)

Creates a direct-access data provider.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    directInfo info: UnsafeMutableRawPointer?,
    size: off_t,
    callbacks: UnsafePointer
)
```

## Parameters 

`info`  

A pointer to data of any type or `NULL`. When Core Graphics calls the functions specified in the `callbacks` parameter, it sends each of the functions this pointer.

`size`  

The number of bytes of data to provide.

`callbacks`  

A pointer to a CGDataProviderDirectCallbacks structure that specifies the callback functions you implement to handle the data provider’s basic memory management.

## Return Value

A new data provider. In Objective-C, you’re responsible for releasing this object using CGDataProviderRelease.

## Discussion

You use this function to create a direct-access data provider that uses callback functions to read data from your program in a single block.

## See Also

### Creating Direct-Access Data Providers

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

typealias CGDataProviderReleaseBytePointerCallback

A callback function that releases the pointer Core Graphics obtained by calling CGDataProviderGetBytePointerCallback.

typealias CGDataProviderReleaseInfoCallback

A callback function that releases any private data or resources associated with the data provider.

typealias CGDataProviderReleaseDataCallback

A callback function that releases data you supply to the function init(dataInfo:data:size:releaseData:).

