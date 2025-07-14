

- Matter
-  MTRClusterSmokeCOAlarm 

Class

# MTRClusterSmokeCOAlarm

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class MTRClusterSmokeCOAlarm
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatteryAlert(with: MTRReadParams?) -> [String : Any]?

func readAttributeCOState(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeContaminationState(with: MTRReadParams?) -> [String : Any]?

func readAttributeDeviceMuted(with: MTRReadParams?) -> [String : Any]?

func readAttributeEndOfServiceAlert(with: MTRReadParams?) -> [String : Any]?

func readAttributeExpiryDate(with: MTRReadParams?) -> [String : Any]?

func readAttributeExpressedState(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeHardwareFaultAlert(with: MTRReadParams?) -> [String : Any]?

func readAttributeInterconnectCOAlarm(with: MTRReadParams?) -> [String : Any]?

func readAttributeInterconnectSmoke(with: MTRReadParams?) -> [String : Any]?

func readAttributeSmokeSensitivityLevel(with: MTRReadParams?) -> [String : Any]?

func readAttributeSmokeState(with: MTRReadParams?) -> [String : Any]?

func readAttributeTestInProgress(with: MTRReadParams?) -> [String : Any]?

func selfTestRequest(with: MTRSmokeCOAlarmClusterSelfTestRequestParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func selfTestRequest(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeSmokeSensitivityLevel(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeSmokeSensitivityLevel(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

