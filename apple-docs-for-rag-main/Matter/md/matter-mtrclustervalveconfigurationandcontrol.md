

- Matter
-  MTRClusterValveConfigurationAndControl 

Class

# MTRClusterValveConfigurationAndControl

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class MTRClusterValveConfigurationAndControl
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func close(with: MTRValveConfigurationAndControlClusterCloseParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func close(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func open(with: MTRValveConfigurationAndControlClusterOpenParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func open(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAutoCloseTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentLevel(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentState(with: MTRReadParams?) -> [String : Any]?

func readAttributeDefaultOpenDuration(with: MTRReadParams?) -> [String : Any]?

func readAttributeDefaultOpenLevel(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeLevelStep(with: MTRReadParams?) -> [String : Any]?

func readAttributeOpenDuration(with: MTRReadParams?) -> [String : Any]?

func readAttributeRemainingDuration(with: MTRReadParams?) -> [String : Any]?

func readAttributeTargetLevel(with: MTRReadParams?) -> [String : Any]?

func readAttributeTargetState(with: MTRReadParams?) -> [String : Any]?

func readAttributeValveFault(with: MTRReadParams?) -> [String : Any]?

func writeAttributeDefaultOpenDuration(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeDefaultOpenDuration(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeDefaultOpenLevel(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeDefaultOpenLevel(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

