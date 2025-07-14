

- Matter
-  MTRClusterTimeSynchronization 

Class

# MTRClusterTimeSynchronization

Cluster Time Synchronization Accurate time is required for a number of reasons, including scheduling, display and validating security materials.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRClusterTimeSynchronization
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

For all instance methods that take a completion (i.e. command invocations), the completion will be called on the provided queue.

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeDSTOffset(with: MTRReadParams?) -> [String : Any]?

func readAttributeDSTOffsetListMaxSize(with: MTRReadParams?) -> [String : Any]?

func readAttributeDefaultNTP(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeGranularity(with: MTRReadParams?) -> [String : Any]?

func readAttributeLocalTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeNTPServerAvailable(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupportsDNSResolve(with: MTRReadParams?) -> [String : Any]?

func readAttributeTimeSource(with: MTRReadParams?) -> [String : Any]?

func readAttributeTimeZone(with: MTRReadParams?) -> [String : Any]?

func readAttributeTimeZoneDatabase(with: MTRReadParams?) -> [String : Any]?

func readAttributeTimeZoneListMaxSize(with: MTRReadParams?) -> [String : Any]?

func readAttributeTrustedTimeSource(with: MTRReadParams?) -> [String : Any]?

func readAttributeUTCTime(with: MTRReadParams?) -> [String : Any]?

func setDSTOffsetWith(MTRTimeSynchronizationClusterSetDSTOffsetParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func setDefaultNTPWith(MTRTimeSynchronizationClusterSetDefaultNTPParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func setTimeZoneWith(MTRTimeSynchronizationClusterSetTimeZoneParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRTimeSynchronizationClusterSetTimeZoneResponseParams?, (any Error)?) -> Void)

func setTrustedTimeSourceWith(MTRTimeSynchronizationClusterSetTrustedTimeSourceParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func setUTCTimeWith(MTRTimeSynchronizationClusterSetUTCTimeParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

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

