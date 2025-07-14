

- Core Graphics
- CGDataConsumer
-  init(url:) 

Initializer

# init(url:)

Creates a data consumer that writes data to a location specified by a URL.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(url: CFURL)
```

## Parameters 

`url`  

A CFURL object that specifies the data destination.

## Return Value

A new data consumer object. In Objective-C, you’re responsible for releasing this object using CGDataConsumerRelease.

## See Also

### Creating Data Consumers

init?(info: UnsafeMutableRawPointer?, cbks: UnsafePointer&lt;CGDataConsumerCallbacks>)

Creates a data consumer that uses callback functions to write data.

init?(data: CFMutableData)

Creates a data consumer that writes to a CFData object.

struct CGDataConsumerCallbacks

A structure that contains pointers to callback functions that manage the copying of data for a data consumer.

typealias CGDataConsumerPutBytesCallback

Copies data from a Core Graphics-supplied buffer into a data consumer.

typealias CGDataConsumerReleaseInfoCallback

Releases any private data or resources associated with the data consumer.

