

- Core Graphics
- CGDataConsumer
-  init(data:) 

Initializer

# init(data:)

Creates a data consumer that writes to a CFData object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init?(data: CFMutableData)
```

## Parameters 

`data`  

The CFData object to write to.

## Return Value

A new data consumer object. In Objective-C, you’re responsible for releasing this object using CGDataConsumerRelease.

## Discussion

You can use this function when you need to represent Core Graphics data as a CFData type. For example, you might create a CFData object that you then copy to the pasteboard.

## See Also

### Creating Data Consumers

init?(info: UnsafeMutableRawPointer?, cbks: UnsafePointer&lt;CGDataConsumerCallbacks>)

Creates a data consumer that uses callback functions to write data.

init?(url: CFURL)

Creates a data consumer that writes data to a location specified by a URL.

struct CGDataConsumerCallbacks

A structure that contains pointers to callback functions that manage the copying of data for a data consumer.

typealias CGDataConsumerPutBytesCallback

Copies data from a Core Graphics-supplied buffer into a data consumer.

typealias CGDataConsumerReleaseInfoCallback

Releases any private data or resources associated with the data consumer.

