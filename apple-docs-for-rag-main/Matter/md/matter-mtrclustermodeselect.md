

- Matter
-  MTRClusterModeSelect 

Class

# MTRClusterModeSelect

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterModeSelect
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func changeToMode(with: MTRModeSelectClusterChangeToModeParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func changeToMode(with: MTRModeSelectClusterChangeToModeParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeDescription(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeOnMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeStandardNamespace(with: MTRReadParams?) -> [String : Any]?

func readAttributeStartUpMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupportedModes(with: MTRReadParams?) -> [String : Any]?

func writeAttributeOnMode(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeOnMode(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeStartUpMode(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeStartUpMode(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

