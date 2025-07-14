

- Matter
-  MTRClusterThreadNetworkDirectory 

Class

# MTRClusterThreadNetworkDirectory

Cluster Thread Network Directory Manages the names and credentials of Thread networks visible to the user.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRClusterThreadNetworkDirectory
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

For all instance methods that take a completion (i.e. command invocations), the completion will be called on the provided queue.

### Instance Methods

func addNetwork(with: MTRThreadNetworkDirectoryClusterAddNetworkParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func getOperationalDataset(with: MTRThreadNetworkDirectoryClusterGetOperationalDatasetParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRThreadNetworkDirectoryClusterOperationalDatasetResponseParams?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributePreferredExtendedPanID(with: MTRReadParams?) -> [String : Any]?

func readAttributeThreadNetworkTableSize(with: MTRReadParams?) -> [String : Any]?

func readAttributeThreadNetworks(with: MTRReadParams?) -> [String : Any]?

func removeNetwork(with: MTRThreadNetworkDirectoryClusterRemoveNetworkParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func writeAttributePreferredExtendedPanID(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributePreferredExtendedPanID(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

