

- Core Graphics
-  CGDataConsumerReleaseInfoCallback 

Type Alias

# CGDataConsumerReleaseInfoCallback

Releases any private data or resources associated with the data consumer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CGDataConsumerReleaseInfoCallback = (UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`info`  

A generic pointer to private data shared among your callback functions. This is the same pointer you supplied to init(info:cbks:).

## Discussion

When Core Graphics frees a data consumer that has an associated release function, the release function is called.

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

typealias CGDataConsumerPutBytesCallback

Copies data from a Core Graphics-supplied buffer into a data consumer.

