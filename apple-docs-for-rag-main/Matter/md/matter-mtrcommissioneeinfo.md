

- Matter
-  MTRCommissioneeInfo 

Class

# MTRCommissioneeInfo

Information read from the commissionee device during commissioning.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRCommissioneeInfo
```

## Topics

### Instance Properties

var endpointsById: [NSNumber : MTREndpointInfo]?

Endpoint information for all endpoints of the commissionee. Will be present only if readEndpointInformation is set to YES on MTRCommissioningParameters.

var productIdentity: MTRProductIdentity

The product identity (VID / PID) of the commissionee.

var rootEndpoint: MTREndpointInfo?

Endpoint information for the root endpoint of the commissionee. Will be present only if readEndpointInformation is set to YES on MTRCommissioningParameters.

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

