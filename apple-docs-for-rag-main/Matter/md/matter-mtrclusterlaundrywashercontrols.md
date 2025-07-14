

- Matter
-  MTRClusterLaundryWasherControls 

Class

# MTRClusterLaundryWasherControls

Cluster Laundry Washer Controls This cluster supports remotely monitoring and controlling the different types of functionality available to a washing device, such as a washing machine.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRClusterLaundryWasherControls
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

func readAttributeNumberOfRinses(with: MTRReadParams?) -> [String : Any]?

func readAttributeSpinSpeedCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeSpinSpeeds(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupportedRinses(with: MTRReadParams?) -> [String : Any]?

func writeAttributeNumberOfRinses(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeNumberOfRinses(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeSpinSpeedCurrent(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeSpinSpeedCurrent(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

