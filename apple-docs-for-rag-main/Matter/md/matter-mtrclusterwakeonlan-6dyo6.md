

- Matter
-  MTRClusterWakeOnLAN 

Class

# MTRClusterWakeOnLAN

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
class MTRClusterWakeOnLAN
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeMACAddress(with: MTRReadParams?) -> [String : Any]?

func readAttributeLinkLocalAddress(with: MTRReadParams?) -> [String : Any]?

## Relationships

### Inherits From

- MTRGenericCluster

### Inherited By

- MTRClusterWakeOnLan

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

