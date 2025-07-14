

- Matter
-  MTRClusterOvenCavityOperationalState 

Class

# MTRClusterOvenCavityOperationalState

Cluster Oven Cavity Operational State This cluster supports remotely monitoring and, where supported, changing the operational state of an Oven.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRClusterOvenCavityOperationalState
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

For all instance methods that take a completion (i.e. command invocations), the completion will be called on the provided queue.

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCountdownTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentPhase(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeOperationalError(with: MTRReadParams?) -> [String : Any]?

func readAttributeOperationalState(with: MTRReadParams?) -> [String : Any]?

func readAttributeOperationalStateList(with: MTRReadParams?) -> [String : Any]?

func readAttributePhaseList(with: MTRReadParams?) -> [String : Any]?

func start(with: MTROvenCavityOperationalStateClusterStartParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROvenCavityOperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

func start(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROvenCavityOperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

func stop(with: MTROvenCavityOperationalStateClusterStopParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROvenCavityOperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

func stop(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROvenCavityOperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

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

