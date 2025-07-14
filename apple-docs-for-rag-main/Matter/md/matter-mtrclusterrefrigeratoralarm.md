

- Matter
-  MTRClusterRefrigeratorAlarm 

Class

# MTRClusterRefrigeratorAlarm

Cluster Refrigerator Alarm Attributes and commands for configuring the Refrigerator alarm.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRClusterRefrigeratorAlarm
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

The queue is currently unused, but may be used in the future for calling completions for command invocations if commands are added to this cluster.

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeMask(with: MTRReadParams?) -> [String : Any]?

func readAttributeState(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupported(with: MTRReadParams?) -> [String : Any]?

## Relationships

### Inherits From

- MTRGenericCluster

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

