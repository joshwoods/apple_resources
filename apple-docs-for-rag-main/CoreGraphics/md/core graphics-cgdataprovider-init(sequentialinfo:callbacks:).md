

- Core Graphics
- CGDataProvider
-  init(sequentialInfo:callbacks:) 

Initializer

# init(sequentialInfo:callbacks:)

Creates a sequential-access data provider.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    sequentialInfo info: UnsafeMutableRawPointer?,
    callbacks: UnsafePointer
)
```

## Parameters 

`info`  

A pointer to data of any type or `NULL`. When Core Graphics calls the functions specified in the `callbacks` parameter, it sends each of the functions this pointer.

`callbacks`  

A pointer to a CGDataProviderSequentialCallbacks structure that specifies the callback functions you implement to handle the data provider’s basic memory management.

## Return Value

A new data provider. In Objective-C, you’re responsible for releasing this object using CGDataProviderRelease.

## Discussion

You use this function to create a sequential-access data provider that uses callback functions to read data from your program in a single block.

## See Also

### Creating Sequential-Access Data Providers

struct CGDataProviderSequentialCallbacks

Defines a structure containing pointers to client-defined callback functions that manage the sending of data for a sequential-access data provider.

typealias CGDataProviderRewindCallback

A callback function that moves the current position in the data stream back to the beginning.

typealias CGDataProviderGetBytesCallback

A callback function that copies from a provider data stream into a Core Graphics buffer.

typealias CGDataProviderSkipForwardCallback

A callback function that advances the current position in the data stream supplied by the provider.

typealias CGDataProviderReleaseInfoCallback

A callback function that releases any private data or resources associated with the data provider.

