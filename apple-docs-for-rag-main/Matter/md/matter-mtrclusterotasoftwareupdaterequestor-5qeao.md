

- Matter
-  MTRClusterOTASoftwareUpdateRequestor 

Class

# MTRClusterOTASoftwareUpdateRequestor

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
class MTRClusterOTASoftwareUpdateRequestor
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

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

- MTRGenericCluster

### Inherited By

- MTRClusterOtaSoftwareUpdateRequestor

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

