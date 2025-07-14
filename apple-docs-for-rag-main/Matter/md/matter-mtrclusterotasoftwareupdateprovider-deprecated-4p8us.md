

- Matter
-  MTRClusterOtaSoftwareUpdateProvider Deprecated

Class

# MTRClusterOtaSoftwareUpdateProvider

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
class MTRClusterOtaSoftwareUpdateProvider
```

Deprecated

Please use MTRClusterOTASoftwareUpdateProvider

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func applyUpdateRequest(with: MTROtaSoftwareUpdateProviderClusterApplyUpdateRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTROtaSoftwareUpdateProviderClusterApplyUpdateResponseParams?, (any Error)?) -> Void)

func notifyUpdateApplied(with: MTROtaSoftwareUpdateProviderClusterNotifyUpdateAppliedParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func queryImage(with: MTROtaSoftwareUpdateProviderClusterQueryImageParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTROtaSoftwareUpdateProviderClusterQueryImageResponseParams?, (any Error)?) -> Void)

func applyUpdateRequest(with: MTROTASoftwareUpdateProviderClusterApplyUpdateRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROTASoftwareUpdateProviderClusterApplyUpdateResponseParams?, (any Error)?) -> Void)

func notifyUpdateApplied(with: MTROTASoftwareUpdateProviderClusterNotifyUpdateAppliedParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func queryImage(with: MTROTASoftwareUpdateProviderClusterQueryImageParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROTASoftwareUpdateProviderClusterQueryImageResponseParams?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

## Relationships

### Inherits From

- MTRClusterOTASoftwareUpdateProvider

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

