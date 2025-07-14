

- Matter
-  MTRDeviceTypeRevision 

Class

# MTRDeviceTypeRevision

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class MTRDeviceTypeRevision
```

## Topics

### Initializers

init?(deviceTypeID: NSNumber, revision: NSNumber)

init?(coder: NSCoder)

init?(deviceTypeStruct: MTRDescriptorClusterDeviceTypeStruct)

Initializes the receiver based on the values in the specified struct.

### Instance Properties

var deviceTypeID: NSNumber

var deviceTypeRevision: NSNumber

var typeInformation: MTRDeviceType?

Returns the MTRDeviceType corresponding to deviceTypeID, or nil if deviceTypeID does not represent a known device type.

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
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

