

- Matter
-  MTRClusterAccessControl 

Class

# MTRClusterAccessControl

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterAccessControl
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeACL(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAccessControlEntriesPerFabric(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcl(with: MTRReadParams?) -> [String : Any]Deprecated

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeExtension(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeSubjectsPerAccessControlEntry(with: MTRReadParams?) -> [String : Any]?

func readAttributeTargetsPerAccessControlEntry(with: MTRReadParams?) -> [String : Any]?

func writeAttributeACL(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeACL(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeAcl(withValue: [String : Any], expectedValueInterval: NSNumber)Deprecated

func writeAttributeAcl(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)Deprecated

func writeAttributeExtension(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeExtension(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func readAttributeARL(with: MTRReadParams?) -> [String : Any]?

func readAttributeCommissioningARL(with: MTRReadParams?) -> [String : Any]?

func reviewFabricRestrictions(with: MTRAccessControlClusterReviewFabricRestrictionsParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRAccessControlClusterReviewFabricRestrictionsResponseParams?, (any Error)?) -> Void)

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

