

- Core Graphics
-  CGDataConsumerPutBytesCallback 

Type Alias

# CGDataConsumerPutBytesCallback

Copies data from a Core Graphics-supplied buffer into a data consumer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CGDataConsumerPutBytesCallback = (UnsafeMutableRawPointer?, UnsafeRawPointer, Int) -> Int
```

## Parameters 

`info`  

A generic pointer to private data shared among your callback functions. This is the pointer supplied to init(info:cbks:).

`buffer`  

The buffer from which you copy the specified number of bytes.

`count`  

The number of bytes to copy.

## Return Value

The number of bytes copied. If no more data can be written to the consumer, you should return `0`.

## Discussion

When Core Graphics is ready to send data to the consumer, your function is called. It should copy the specified number of bytes from `buffer` into some resource under your control—for example, a file.

For information on how to associate your callback function with a data consumer, see init(info:cbks:) and CGDataConsumerCallbacks.

## See Also

### Creating Data Consumers

init?(info: UnsafeMutableRawPointer?, cbks: UnsafePointer&lt;CGDataConsumerCallbacks>)

Creates a data consumer that uses callback functions to write data.

init?(url: CFURL)

Creates a data consumer that writes data to a location specified by a URL.

init?(data: CFMutableData)

Creates a data consumer that writes to a CFData object.

struct CGDataConsumerCallbacks

A structure that contains pointers to callback functions that manage the copying of data for a data consumer.

typealias CGDataConsumerReleaseInfoCallback

Releases any private data or resources associated with the data consumer.

