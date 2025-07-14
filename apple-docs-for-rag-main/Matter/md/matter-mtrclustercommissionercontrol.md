

- Matter
-  MTRClusterCommissionerControl 

Class

# MTRClusterCommissionerControl

Cluster Commissioner Control Supports the ability for clients to request the commissioning of themselves or other nodes onto a fabric which the cluster server can commission onto.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRClusterCommissionerControl
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

For all instance methods that take a completion (i.e. command invocations), the completion will be called on the provided queue.

### Instance Methods

func commissionNode(with: MTRCommissionerControlClusterCommissionNodeParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRCommissionerControlClusterReverseOpenCommissioningWindowParams?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupportedDeviceCategories(with: MTRReadParams?) -> [String : Any]?

func requestCommissioningApproval(with: MTRCommissionerControlClusterRequestCommissioningApprovalParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

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

