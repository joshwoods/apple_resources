

- Matter
-  MTRServerEndpoint 

Class

# MTRServerEndpoint

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class MTRServerEndpoint
```

## Topics

### Initializers

init?(endpointID: NSNumber, deviceTypes: [MTRDeviceTypeRevision])

### Instance Properties

var accessGrants: [MTRAccessGrant]

var deviceTypes: [MTRDeviceTypeRevision]

var endpointID: NSNumber

var serverClusters: [MTRServerCluster]

### Instance Methods

func addAccessGrant(MTRAccessGrant)

func addServerCluster(MTRServerCluster) -> Bool

func removeAccessGrant(MTRAccessGrant)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

