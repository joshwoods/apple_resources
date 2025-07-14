

- Matter
-  MTRClusterOTASoftwareUpdateProvider 

Class

# MTRClusterOTASoftwareUpdateProvider

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
class MTRClusterOTASoftwareUpdateProvider
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

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

- MTRGenericCluster

### Inherited By

- MTRClusterOtaSoftwareUpdateProvider

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

