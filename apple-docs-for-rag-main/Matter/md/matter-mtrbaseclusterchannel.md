

- Matter
-  MTRBaseClusterChannel 

Class

# MTRBaseClusterChannel

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRBaseClusterChannel
```

## Topics

### Initializers

init?(device: MTRBaseDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRBaseDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func change(with: MTRChannelClusterChangeChannelParams, completion: (MTRChannelClusterChangeChannelResponseParams?, (any Error)?) -> Void)

func change(with: MTRChannelClusterChangeChannelParams, completionHandler: (MTRChannelClusterChangeChannelResponseParams?, (any Error)?) -> Void)Deprecated

func changeByNumber(with: MTRChannelClusterChangeChannelByNumberParams, completion: MTRStatusCompletion)

func changeByNumber(with: MTRChannelClusterChangeChannelByNumberParams, completionHandler: MTRStatusCompletion)Deprecated

func readAttributeAcceptedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeAttributeList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAttributeList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeChannelList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeChannelList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeClusterRevision(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeClusterRevision(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeCurrentChannel(completion: (MTRChannelClusterChannelInfoStruct?, (any Error)?) -> Void)

func readAttributeCurrentChannel(completionHandler: (MTRChannelClusterChannelInfo?, (any Error)?) -> Void)Deprecated

func readAttributeFeatureMap(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFeatureMap(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeGeneratedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeLineup(completion: (MTRChannelClusterLineupInfoStruct?, (any Error)?) -> Void)

func readAttributeLineup(completionHandler: (MTRChannelClusterLineupInfo?, (any Error)?) -> Void)Deprecated

func skip(with: MTRChannelClusterSkipChannelParams, completion: MTRStatusCompletion)

func skip(with: MTRChannelClusterSkipChannelParams, completionHandler: MTRStatusCompletion)Deprecated

func subscribeAttributeAcceptedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAttributeList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeChannelList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeChannelList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeClusterRevision(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeCurrentChannel(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (MTRChannelClusterChannelInfoStruct?, (any Error)?) -> Void)

func subscribeAttributeCurrentChannel(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (MTRChannelClusterChannelInfo?, (any Error)?) -> Void)Deprecated

func subscribeAttributeFeatureMap(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeGeneratedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLineup(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (MTRChannelClusterLineupInfoStruct?, (any Error)?) -> Void)

func subscribeAttributeLineup(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (MTRChannelClusterLineupInfo?, (any Error)?) -> Void)Deprecated

func cancelRecordProgram(with: MTRChannelClusterCancelRecordProgramParams, completion: MTRStatusCompletion)

Command CancelRecordProgram

func getProgramGuide(completion: (MTRChannelClusterProgramGuideResponseParams?, (any Error)?) -> Void)

func getProgramGuide(with: MTRChannelClusterGetProgramGuideParams?, completion: (MTRChannelClusterProgramGuideResponseParams?, (any Error)?) -> Void)

Command GetProgramGuide

func recordProgram(with: MTRChannelClusterRecordProgramParams, completion: MTRStatusCompletion)

Command RecordProgram

### Type Methods

class func readAttributeAcceptedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAcceptedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeAttributeList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAttributeList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeChannelList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeChannelList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeClusterRevision(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeCurrentChannel(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (MTRChannelClusterChannelInfo?, (any Error)?) -> Void)Deprecated

class func readAttributeCurrentChannel(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (MTRChannelClusterChannelInfoStruct?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeFeatureMap(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeGeneratedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeLineup(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (MTRChannelClusterLineupInfo?, (any Error)?) -> Void)Deprecated

class func readAttributeLineup(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (MTRChannelClusterLineupInfoStruct?, (any Error)?) -> Void)

## Relationships

### Inherits From

- MTRGenericBaseCluster

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

