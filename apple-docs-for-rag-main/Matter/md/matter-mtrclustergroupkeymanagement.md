

- Matter
-  MTRClusterGroupKeyManagement 

Class

# MTRClusterGroupKeyManagement

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterGroupKeyManagement
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func keySetRead(with: MTRGroupKeyManagementClusterKeySetReadParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRGroupKeyManagementClusterKeySetReadResponseParams?, (any Error)?) -> Void)

func keySetRead(with: MTRGroupKeyManagementClusterKeySetReadParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRGroupKeyManagementClusterKeySetReadResponseParams?, (any Error)?) -> Void)Deprecated

func keySetReadAllIndices(with: MTRGroupKeyManagementClusterKeySetReadAllIndicesParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRGroupKeyManagementClusterKeySetReadAllIndicesResponseParams?, (any Error)?) -> Void)

func keySetReadAllIndices(with: MTRGroupKeyManagementClusterKeySetReadAllIndicesParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRGroupKeyManagementClusterKeySetReadAllIndicesResponseParams?, (any Error)?) -> Void)Deprecated

func keySetReadAllIndices(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRGroupKeyManagementClusterKeySetReadAllIndicesResponseParams?, (any Error)?) -> Void)

func keySetRemove(with: MTRGroupKeyManagementClusterKeySetRemoveParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func keySetRemove(with: MTRGroupKeyManagementClusterKeySetRemoveParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func keySetWrite(with: MTRGroupKeyManagementClusterKeySetWriteParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func keySetWrite(with: MTRGroupKeyManagementClusterKeySetWriteParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeGroupKeyMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGroupTable(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxGroupKeysPerFabric(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxGroupsPerFabric(with: MTRReadParams?) -> [String : Any]?

func writeAttributeGroupKeyMap(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeGroupKeyMap(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

