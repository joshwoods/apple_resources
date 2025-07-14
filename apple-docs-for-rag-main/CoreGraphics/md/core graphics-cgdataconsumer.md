

- Core Graphics
-  CGDataConsumer 

Class

# CGDataConsumer

An abstraction for data-writing tasks that eliminates the need to manage a raw memory buffer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CGDataConsumer
```

## Overview

Most apps should use CGImageDestination objects instead.

## Topics

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

typealias CGDataConsumerReleaseInfoCallback

Releases any private data or resources associated with the data consumer.

### Working with Core Foundation Types

class var typeID: CFTypeID

Returns the Core Foundation type identifier for Core Graphics data consumers.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Quartz 2D Programming Guide

### Utility and Support Classes

class CGDataProvider

An abstraction for data-reading tasks that eliminates the need to manage a raw memory buffer.

class CGShading

A definition for a smooth transition between colors, controlled by a custom function you provide, for drawing radial and axial gradient fills.

class CGGradient

A definition for a smooth transition between colors for drawing radial and axial gradient fills.

class CGFunction

A general facility for defining and using callback functions.

class CGPattern

A 2D pattern to be used for drawing graphics paths.

