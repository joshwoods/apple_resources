

- Matter
-  MTREndpointInfo 

Class

# MTREndpointInfo

Meta-data about an endpoint of a Matter node.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTREndpointInfo
```

## Topics

### Instance Properties

var children: [MTREndpointInfo]

The direct children of this endpoint. This excludes indirect descendants even if they are listed in the PartsList attribute of this endpoint due to the Full-Family Pattern being used. Refer to Endpoint Composition Patterns in the Matter specification for details.

var deviceTypes: [MTRDeviceTypeRevision]

var endpointID: NSNumber

var partsList: [NSNumber]

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

