

- Matter
-  MTRClusterLevelControl 

Class

# MTRClusterLevelControl

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterLevelControl
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func move(with: MTRLevelControlClusterMoveParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func move(with: MTRLevelControlClusterMoveParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func moveToClosestFrequency(with: MTRLevelControlClusterMoveToClosestFrequencyParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func moveToClosestFrequency(with: MTRLevelControlClusterMoveToClosestFrequencyParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func moveToLevel(with: MTRLevelControlClusterMoveToLevelParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func moveToLevel(with: MTRLevelControlClusterMoveToLevelParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func moveToLevelWithOnOff(with: MTRLevelControlClusterMoveToLevelWithOnOffParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func moveToLevelWithOnOff(with: MTRLevelControlClusterMoveToLevelWithOnOffParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func moveWithOnOff(with: MTRLevelControlClusterMoveWithOnOffParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func moveWithOnOff(with: MTRLevelControlClusterMoveWithOnOffParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentFrequency(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentLevel(with: MTRReadParams?) -> [String : Any]?

func readAttributeDefaultMoveRate(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxFrequency(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxLevel(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinFrequency(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinLevel(with: MTRReadParams?) -> [String : Any]?

func readAttributeOffTransitionTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeOnLevel(with: MTRReadParams?) -> [String : Any]?

func readAttributeOnOffTransitionTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeOnTransitionTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeOptions(with: MTRReadParams?) -> [String : Any]?

func readAttributeRemainingTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeStartUpCurrentLevel(with: MTRReadParams?) -> [String : Any]?

func step(with: MTRLevelControlClusterStepParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func step(with: MTRLevelControlClusterStepParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func stepWithOnOff(with: MTRLevelControlClusterStepWithOnOffParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func stepWithOnOff(with: MTRLevelControlClusterStepWithOnOffParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func stop(with: MTRLevelControlClusterStopParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func stop(with: MTRLevelControlClusterStopParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func stopWithOnOff(with: MTRLevelControlClusterStopWithOnOffParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func stopWithOnOff(with: MTRLevelControlClusterStopWithOnOffParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeDefaultMoveRate(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeDefaultMoveRate(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeOffTransitionTime(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeOffTransitionTime(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeOnLevel(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeOnLevel(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeOnOffTransitionTime(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeOnOffTransitionTime(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeOnTransitionTime(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeOnTransitionTime(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeOptions(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeOptions(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeStartUpCurrentLevel(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeStartUpCurrentLevel(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

