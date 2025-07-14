

- Matter
-  MTRClusterRVCRunMode 

Class

# MTRClusterRVCRunMode

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
class MTRClusterRVCRunMode
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func changeToMode(with: MTRRVCRunModeClusterChangeToModeParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRRVCRunModeClusterChangeToModeResponseParams?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupportedModes(with: MTRReadParams?) -> [String : Any]?

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

