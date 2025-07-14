

- Core Graphics
- CGDataProvider
-  init(dataInfo:data:size:releaseData:) 

Initializer

# init(dataInfo:data:size:releaseData:)

Creates a direct-access data provider that uses data your program supplies.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    dataInfo info: UnsafeMutableRawPointer?,
    data: UnsafeRawPointer,
    size: Int,
    releaseData: CGDataProviderReleaseDataCallback
)
```

## Parameters 

`info`  

A pointer to data of any type, or `NULL`. When Core Graphics calls the function specified in the `releaseData` parameter, it sends this pointer as its first argument.

`data`  

A pointer to the array of data that the provider contains.

`size`  

A value that specifies the number of bytes that the data provider contains.

`releaseData`  

A pointer to a release callback for the data provider, or `NULL`. Your release function is called when Core Graphics frees the data provider. For more information, see CGDataProviderReleaseDataCallback.

## Return Value

A new data provider. In Objective-C, you’re responsible for releasing this object using CGDataProviderRelease.

## Discussion

You use this function to create a direct-access data provider that uses callback functions to read data from your program an entire block at one time.

## See Also

### Creating Direct-Access Data Providers

init?(directInfo: UnsafeMutableRawPointer?, size: off_t, callbacks: UnsafePointer&lt;CGDataProviderDirectCallbacks>)

Creates a direct-access data provider.

init?(data: CFData)

Creates a data provider that reads from a CFData object.

init?(url: CFURL)

Creates a direct-access data provider that uses a URL to supply data.

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

