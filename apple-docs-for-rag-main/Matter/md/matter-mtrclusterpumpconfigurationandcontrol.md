

- Matter
-  MTRClusterPumpConfigurationAndControl 

Class

# MTRClusterPumpConfigurationAndControl

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterPumpConfigurationAndControl
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeCapacity(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeControlMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeEffectiveControlMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeEffectiveOperationMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeLifetimeEnergyConsumed(with: MTRReadParams?) -> [String : Any]?

func readAttributeLifetimeRunningHours(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxCompPressure(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxConstFlow(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxConstPressure(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxConstSpeed(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxConstTemp(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxFlow(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxPressure(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxSpeed(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinCompPressure(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinConstFlow(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinConstPressure(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinConstSpeed(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinConstTemp(with: MTRReadParams?) -> [String : Any]?

func readAttributeOperationMode(with: MTRReadParams?) -> [String : Any]?

func readAttributePower(with: MTRReadParams?) -> [String : Any]?

func readAttributePumpStatus(with: MTRReadParams?) -> [String : Any]?

func readAttributeSpeed(with: MTRReadParams?) -> [String : Any]?

func writeAttributeControlMode(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeControlMode(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeLifetimeEnergyConsumed(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeLifetimeEnergyConsumed(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeLifetimeRunningHours(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeLifetimeRunningHours(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeOperationMode(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeOperationMode(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

