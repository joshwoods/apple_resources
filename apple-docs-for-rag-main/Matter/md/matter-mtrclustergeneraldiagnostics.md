

- Matter
-  MTRClusterGeneralDiagnostics 

Class

# MTRClusterGeneralDiagnostics

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterGeneralDiagnostics
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeActiveHardwareFaults(with: MTRReadParams?) -> [String : Any]?

func readAttributeActiveNetworkFaults(with: MTRReadParams?) -> [String : Any]?

func readAttributeActiveRadioFaults(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeBootReason(with: MTRReadParams?) -> [String : Any]?

func readAttributeBootReasons(with: MTRReadParams?) -> [String : Any]Deprecated

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeNetworkInterfaces(with: MTRReadParams?) -> [String : Any]?

func readAttributeRebootCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTestEventTriggersEnabled(with: MTRReadParams?) -> [String : Any]?

func readAttributeTotalOperationalHours(with: MTRReadParams?) -> [String : Any]?

func readAttributeUpTime(with: MTRReadParams?) -> [String : Any]?

func testEventTrigger(with: MTRGeneralDiagnosticsClusterTestEventTriggerParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func testEventTrigger(with: MTRGeneralDiagnosticsClusterTestEventTriggerParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func payloadTestRequest(with: MTRGeneralDiagnosticsClusterPayloadTestRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRGeneralDiagnosticsClusterPayloadTestResponseParams?, (any Error)?) -> Void)

func timeSnapshot(with: MTRGeneralDiagnosticsClusterTimeSnapshotParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRGeneralDiagnosticsClusterTimeSnapshotResponseParams?, (any Error)?) -> Void)

func timeSnapshot(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRGeneralDiagnosticsClusterTimeSnapshotResponseParams?, (any Error)?) -> Void)

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

