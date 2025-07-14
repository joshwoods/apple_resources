

- Matter
-  MTRClusterRVCOperationalState 

Class

# MTRClusterRVCOperationalState

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
class MTRClusterRVCOperationalState
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func pause(with: MTRRVCOperationalStateClusterPauseParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRRVCOperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

func pause(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRRVCOperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

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

func resume(with: MTRRVCOperationalStateClusterResumeParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRRVCOperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

func resume(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRRVCOperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

func goHome(with: MTRRVCOperationalStateClusterGoHomeParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRRVCOperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

func goHome(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRRVCOperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void)

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

