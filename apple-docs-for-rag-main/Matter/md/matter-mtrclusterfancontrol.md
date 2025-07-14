

- Matter
-  MTRClusterFanControl 

Class

# MTRClusterFanControl

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterFanControl
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAirflowDirection(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFanMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeFanModeSequence(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributePercentCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributePercentSetting(with: MTRReadParams?) -> [String : Any]?

func readAttributeRockSetting(with: MTRReadParams?) -> [String : Any]?

func readAttributeRockSupport(with: MTRReadParams?) -> [String : Any]?

func readAttributeSpeedCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeSpeedMax(with: MTRReadParams?) -> [String : Any]?

func readAttributeSpeedSetting(with: MTRReadParams?) -> [String : Any]?

func readAttributeWindSetting(with: MTRReadParams?) -> [String : Any]?

func readAttributeWindSupport(with: MTRReadParams?) -> [String : Any]?

func step(with: MTRFanControlClusterStepParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeAirflowDirection(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeAirflowDirection(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeFanMode(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeFanMode(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeFanModeSequence(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeFanModeSequence(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributePercentSetting(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributePercentSetting(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeRockSetting(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeRockSetting(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeSpeedSetting(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeSpeedSetting(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeWindSetting(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeWindSetting(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

