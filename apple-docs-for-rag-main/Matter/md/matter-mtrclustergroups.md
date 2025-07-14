

- Matter
-  MTRClusterGroups 

Class

# MTRClusterGroups

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterGroups
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func addGroup(with: MTRGroupsClusterAddGroupParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRGroupsClusterAddGroupResponseParams?, (any Error)?) -> Void)

func addGroup(with: MTRGroupsClusterAddGroupParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRGroupsClusterAddGroupResponseParams?, (any Error)?) -> Void)Deprecated

func addGroupIfIdentifying(with: MTRGroupsClusterAddGroupIfIdentifyingParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func addGroupIfIdentifying(with: MTRGroupsClusterAddGroupIfIdentifyingParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func getGroupMembership(with: MTRGroupsClusterGetGroupMembershipParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRGroupsClusterGetGroupMembershipResponseParams?, (any Error)?) -> Void)

func getGroupMembership(with: MTRGroupsClusterGetGroupMembershipParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRGroupsClusterGetGroupMembershipResponseParams?, (any Error)?) -> Void)Deprecated

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeNameSupport(with: MTRReadParams?) -> [String : Any]?

func removeAllGroups(with: MTRGroupsClusterRemoveAllGroupsParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func removeAllGroups(with: MTRGroupsClusterRemoveAllGroupsParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func removeAllGroups(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func removeAllGroups(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func removeGroup(with: MTRGroupsClusterRemoveGroupParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRGroupsClusterRemoveGroupResponseParams?, (any Error)?) -> Void)

func removeGroup(with: MTRGroupsClusterRemoveGroupParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRGroupsClusterRemoveGroupResponseParams?, (any Error)?) -> Void)Deprecated

func viewGroup(with: MTRGroupsClusterViewGroupParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRGroupsClusterViewGroupResponseParams?, (any Error)?) -> Void)

func viewGroup(with: MTRGroupsClusterViewGroupParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRGroupsClusterViewGroupResponseParams?, (any Error)?) -> Void)Deprecated

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

