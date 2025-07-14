

- Matter
-  MTRServerCluster 

Class

# MTRServerCluster

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class MTRServerCluster
```

## Topics

### Initializers

init?(clusterID: NSNumber, revision: NSNumber)

### Instance Properties

var accessGrants: [MTRAccessGrant]

var attributes: [MTRServerAttribute]

var clusterID: NSNumber

var clusterRevision: NSNumber

### Instance Methods

func addAccessGrant(MTRAccessGrant)

func addAttribute(MTRServerAttribute) -> Bool

func removeAccessGrant(MTRAccessGrant)

### Type Methods

class func newDescriptor() -> Self

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

