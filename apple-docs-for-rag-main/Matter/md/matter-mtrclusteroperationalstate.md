

- Matter
-  MTRClusterOperationalState 

Class

# MTRClusterOperationalState

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
class MTRClusterOperationalState
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func pause(with: MTROperationalStateClusterPauseParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

func pause(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

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

func resume(with: MTROperationalStateClusterResumeParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

func resume(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

func start(with: MTROperationalStateClusterStartParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

func start(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

func stop(with: MTROperationalStateClusterStopParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

func stop(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

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

