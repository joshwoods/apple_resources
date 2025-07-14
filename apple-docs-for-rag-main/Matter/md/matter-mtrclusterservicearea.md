

- Matter
-  MTRClusterServiceArea 

Class

# MTRClusterServiceArea

Cluster Service Area The Service Area cluster provides an interface for controlling the areas where a device should operate, and for querying the current area being serviced.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRClusterServiceArea
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

For all instance methods that take a completion (i.e. command invocations), the completion will be called on the provided queue.

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentArea(with: MTRReadParams?) -> [String : Any]?

func readAttributeEstimatedEndTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeProgress(with: MTRReadParams?) -> [String : Any]?

func readAttributeSelectedAreas(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupportedAreas(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupportedMaps(with: MTRReadParams?) -> [String : Any]?

func selectAreas(with: MTRServiceAreaClusterSelectAreasParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRServiceAreaClusterSelectAreasResponseParams?, (any Error)?) -> Void)

func skip(with: MTRServiceAreaClusterSkipAreaParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRServiceAreaClusterSkipAreaResponseParams?, (any Error)?) -> Void)

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

