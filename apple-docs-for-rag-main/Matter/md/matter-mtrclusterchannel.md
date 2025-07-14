

- Matter
-  MTRClusterChannel 

Class

# MTRClusterChannel

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterChannel
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func change(with: MTRChannelClusterChangeChannelParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRChannelClusterChangeChannelResponseParams?, (any Error)?) -> Void)

func change(with: MTRChannelClusterChangeChannelParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRChannelClusterChangeChannelResponseParams?, (any Error)?) -> Void)Deprecated

func changeByNumber(with: MTRChannelClusterChangeChannelByNumberParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func changeByNumber(with: MTRChannelClusterChangeChannelByNumberParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeChannelList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentChannel(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeLineup(with: MTRReadParams?) -> [String : Any]?

func skip(with: MTRChannelClusterSkipChannelParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func skip(with: MTRChannelClusterSkipChannelParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func cancelRecordProgram(with: MTRChannelClusterCancelRecordProgramParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func getProgramGuide(with: MTRChannelClusterGetProgramGuideParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRChannelClusterProgramGuideResponseParams?, (any Error)?) -> Void)

func getProgramGuide(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRChannelClusterProgramGuideResponseParams?, (any Error)?) -> Void)

func recordProgram(with: MTRChannelClusterRecordProgramParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

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

