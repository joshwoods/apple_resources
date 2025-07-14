

- Matter
-  MTRClusterActions 

Class

# MTRClusterActions

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterActions
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func disableAction(with: MTRActionsClusterDisableActionParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func disableAction(with: MTRActionsClusterDisableActionParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func disableActionWithDuration(with: MTRActionsClusterDisableActionWithDurationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func disableActionWithDuration(with: MTRActionsClusterDisableActionWithDurationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func enableAction(with: MTRActionsClusterEnableActionParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func enableAction(with: MTRActionsClusterEnableActionParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func enableActionWithDuration(with: MTRActionsClusterEnableActionWithDurationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func enableActionWithDuration(with: MTRActionsClusterEnableActionWithDurationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func instantAction(with: MTRActionsClusterInstantActionParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func instantAction(with: MTRActionsClusterInstantActionParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func instantActionWithTransition(with: MTRActionsClusterInstantActionWithTransitionParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func instantActionWithTransition(with: MTRActionsClusterInstantActionWithTransitionParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func pauseAction(with: MTRActionsClusterPauseActionParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func pauseAction(with: MTRActionsClusterPauseActionParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func pauseActionWithDuration(with: MTRActionsClusterPauseActionWithDurationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func pauseActionWithDuration(with: MTRActionsClusterPauseActionWithDurationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeActionList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeEndpointLists(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeSetupURL(with: MTRReadParams?) -> [String : Any]?

func resumeAction(with: MTRActionsClusterResumeActionParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func resumeAction(with: MTRActionsClusterResumeActionParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func startAction(with: MTRActionsClusterStartActionParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func startAction(with: MTRActionsClusterStartActionParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func startActionWithDuration(with: MTRActionsClusterStartActionWithDurationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func startActionWithDuration(with: MTRActionsClusterStartActionWithDurationParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func stopAction(with: MTRActionsClusterStopActionParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func stopAction(with: MTRActionsClusterStopActionParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

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

