

- Matter
-  MTRClusterOtaSoftwareUpdateRequestor Deprecated

Class

# MTRClusterOtaSoftwareUpdateRequestor

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
class MTRClusterOtaSoftwareUpdateRequestor
```

Deprecated

Please use MTRClusterOTASoftwareUpdateRequestor

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func announceOtaProvider(with: MTROtaSoftwareUpdateRequestorClusterAnnounceOtaProviderParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func readAttributeDefaultOtaProviders(with: MTRReadParams?) -> [String : Any]

func writeAttributeDefaultOtaProviders(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeDefaultOtaProviders(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func announceOTAProvider(with: MTROTASoftwareUpdateRequestorClusterAnnounceOTAProviderParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeDefaultOTAProviders(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeUpdatePossible(with: MTRReadParams?) -> [String : Any]?

func readAttributeUpdateState(with: MTRReadParams?) -> [String : Any]?

func readAttributeUpdateStateProgress(with: MTRReadParams?) -> [String : Any]?

func writeAttributeDefaultOTAProviders(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeDefaultOTAProviders(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

## Relationships

### Inherits From

- MTRClusterOTASoftwareUpdateRequestor

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

