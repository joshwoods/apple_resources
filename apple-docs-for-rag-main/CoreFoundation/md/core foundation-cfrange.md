

- Core Foundation
-  CFRange 

Structure

# CFRange

A structure representing a range of sequential items in a container, such as characters in a buffer or elements in a collection.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFRange
```

## Topics

### Initializers

init()

init(location: CFIndex, length: CFIndex)

### Instance Properties

var length: CFIndex

An integer representing the number of items in the range. For type compatibility with the rest of the system, `LONG_MAX` is the maximum value you should use for length.

var location: CFIndex

An integer representing the starting location of the range. For type compatibility with the rest of the system, `LONG_MAX` is the maximum value you should use for location.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

typealias CFIndex

Priority values used for kAXPriorityKey

typealias CFOptionFlags

A bitfield used for passing special allocation and other requests into Core Foundation functions.

