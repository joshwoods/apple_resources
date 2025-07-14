

- Matter
-  MTRDeviceType 

Class

# MTRDeviceType

Meta-data about a device type defined in the Matter specification.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
class MTRDeviceType
```

## Topics

### Initializers

init?(forID: NSNumber)

Returns an MTRDeviceType for the given ID, if the ID is known. Returns nil for unknown IDs.

### Instance Properties

var id: NSNumber

The identifier of the device type (32-bit unsigned integer).

var isUtility: Bool

Returns whether this is a utility device type.

var name: String

Returns the name of the device type.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

