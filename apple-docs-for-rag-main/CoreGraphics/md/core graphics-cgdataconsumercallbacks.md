

- Core Graphics
-  CGDataConsumerCallbacks 

Structure

# CGDataConsumerCallbacks

A structure that contains pointers to callback functions that manage the copying of data for a data consumer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CGDataConsumerCallbacks
```

## Overview

The functions specified by the `CGDataConsumerCallbacks` structure are responsible for copying data that Core Graphics sends to your consumer and for handling the consumer’s basic memory management. You supply this structure to the function init(info:cbks:) to create a data consumer.

## Topics

### Initializers

init()

init(putBytes: CGDataConsumerPutBytesCallback?, releaseConsumer: CGDataConsumerReleaseInfoCallback?)

### Instance Properties

var putBytes: CGDataConsumerPutBytesCallback?

A pointer to a function that copies data to the data consumer. For more information, see CGDataConsumerPutBytesCallback.

var releaseConsumer: CGDataConsumerReleaseInfoCallback?

A pointer to a function that handles clean-up for the data consumer, or `NULL`.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Creating Data Consumers

init?(info: UnsafeMutableRawPointer?, cbks: UnsafePointer&lt;CGDataConsumerCallbacks>)

Creates a data consumer that uses callback functions to write data.

init?(url: CFURL)

Creates a data consumer that writes data to a location specified by a URL.

init?(data: CFMutableData)

Creates a data consumer that writes to a CFData object.

typealias CGDataConsumerPutBytesCallback

Copies data from a Core Graphics-supplied buffer into a data consumer.

typealias CGDataConsumerReleaseInfoCallback

Releases any private data or resources associated with the data consumer.

