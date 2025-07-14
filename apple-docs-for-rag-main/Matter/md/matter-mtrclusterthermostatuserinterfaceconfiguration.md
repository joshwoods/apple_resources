

- Matter
-  MTRClusterThermostatUserInterfaceConfiguration 

Class

# MTRClusterThermostatUserInterfaceConfiguration

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterThermostatUserInterfaceConfiguration
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeKeypadLockout(with: MTRReadParams?) -> [String : Any]?

func readAttributeScheduleProgrammingVisibility(with: MTRReadParams?) -> [String : Any]?

func readAttributeTemperatureDisplayMode(with: MTRReadParams?) -> [String : Any]?

func writeAttributeKeypadLockout(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeKeypadLockout(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeScheduleProgrammingVisibility(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeScheduleProgrammingVisibility(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeTemperatureDisplayMode(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeTemperatureDisplayMode(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

