

- Core Graphics
- CGDataConsumer
-  init(info:cbks:) 

Initializer

# init(info:cbks:)

Creates a data consumer that uses callback functions to write data.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(
    info: UnsafeMutableRawPointer?,
    cbks: UnsafePointer
)
```

## Parameters 

`info`  

A pointer to data of any type or `NULL`. When the callback is called, Core Graphics passes this pointer as the `info` parameter.

`cbks`  

A pointer to a structure that specifies the callback functions you implement to copy data sent to the consumer and to handle the consumer’s basic memory management. For a complete description, see CGDataConsumerCallbacks.

## Return Value

A new data consumer object. In Objective-C, you’re responsible for releasing this object using CGDataConsumerRelease.

## See Also

### Creating Data Consumers

init?(url: CFURL)

Creates a data consumer that writes data to a location specified by a URL.

init?(data: CFMutableData)

Creates a data consumer that writes to a CFData object.

struct CGDataConsumerCallbacks

A structure that contains pointers to callback functions that manage the copying of data for a data consumer.

typealias CGDataConsumerPutBytesCallback

Copies data from a Core Graphics-supplied buffer into a data consumer.

typealias CGDataConsumerReleaseInfoCallback

Releases any private data or resources associated with the data consumer.

