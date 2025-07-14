

- Matter
-  MTRClusterThreadBorderRouterManagement 

Class

# MTRClusterThreadBorderRouterManagement

Cluster Thread Border Router Management Manage the Thread network of Thread Border Router

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRClusterThreadBorderRouterManagement
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

For all instance methods that take a completion (i.e. command invocations), the completion will be called on the provided queue.

### Instance Methods

func getActiveDatasetRequest(with: MTRThreadBorderRouterManagementClusterGetActiveDatasetRequestParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRThreadBorderRouterManagementClusterDatasetResponseParams?, (any Error)?) -> Void)

func getActiveDatasetRequest(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRThreadBorderRouterManagementClusterDatasetResponseParams?, (any Error)?) -> Void)

func getPendingDatasetRequest(with: MTRThreadBorderRouterManagementClusterGetPendingDatasetRequestParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRThreadBorderRouterManagementClusterDatasetResponseParams?, (any Error)?) -> Void)

func getPendingDatasetRequest(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRThreadBorderRouterManagementClusterDatasetResponseParams?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeActiveDatasetTimestamp(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeBorderAgentID(with: MTRReadParams?) -> [String : Any]?

func readAttributeBorderRouterName(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeInterfaceEnabled(with: MTRReadParams?) -> [String : Any]?

func readAttributePendingDatasetTimestamp(with: MTRReadParams?) -> [String : Any]?

func readAttributeThreadVersion(with: MTRReadParams?) -> [String : Any]?

func setActiveDatasetRequestWith(MTRThreadBorderRouterManagementClusterSetActiveDatasetRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func setPendingDatasetRequestWith(MTRThreadBorderRouterManagementClusterSetPendingDatasetRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

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

