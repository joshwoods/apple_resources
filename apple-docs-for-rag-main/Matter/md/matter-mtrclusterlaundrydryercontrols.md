

- Matter
-  MTRClusterLaundryDryerControls 

Class

# MTRClusterLaundryDryerControls

Cluster Laundry Dryer Controls This cluster provides a way to access options associated with the operation of a laundry dryer device type.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRClusterLaundryDryerControls
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

func readAttributeSelectedDrynessLevel(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupportedDrynessLevels(with: MTRReadParams?) -> [String : Any]?

func writeAttributeSelectedDrynessLevel(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeSelectedDrynessLevel(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

