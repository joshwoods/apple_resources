

- Matter
-  MTRClusterICDManagement 

Class

# MTRClusterICDManagement

Cluster ICD Management Allows servers to ensure that listed clients are notified when a server is available for communication.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRClusterICDManagement
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

For all instance methods that take a completion (i.e. command invocations), the completion will be called on the provided queue.

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeActiveModeDuration(with: MTRReadParams?) -> [String : Any]?

func readAttributeActiveModeThreshold(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClientsSupportedPerFabric(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeICDCounter(with: MTRReadParams?) -> [String : Any]?

func readAttributeIdleModeDuration(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaximumCheckInBackOff(with: MTRReadParams?) -> [String : Any]?

func readAttributeOperatingMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeRegisteredClients(with: MTRReadParams?) -> [String : Any]?

func readAttributeUserActiveModeTriggerHint(with: MTRReadParams?) -> [String : Any]?

func readAttributeUserActiveModeTriggerInstruction(with: MTRReadParams?) -> [String : Any]?

func registerClient(with: MTRICDManagementClusterRegisterClientParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRICDManagementClusterRegisterClientResponseParams?, (any Error)?) -> Void)

func stayActiveRequest(with: MTRICDManagementClusterStayActiveRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRICDManagementClusterStayActiveResponseParams?, (any Error)?) -> Void)

func unregisterClient(with: MTRICDManagementClusterUnregisterClientParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

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

