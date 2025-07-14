

- Matter
-  MTRBaseClusterMediaPlayback 

Class

# MTRBaseClusterMediaPlayback

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRBaseClusterMediaPlayback
```

## Topics

### Initializers

init?(device: MTRBaseDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRBaseDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func fastForward(completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func fastForward(completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func fastForward(with: MTRMediaPlaybackClusterFastForwardParams?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func fastForward(with: MTRMediaPlaybackClusterFastForwardParams?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func next(completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func next(completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func next(with: MTRMediaPlaybackClusterNextParams?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func next(with: MTRMediaPlaybackClusterNextParams?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func pause(completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func pause(completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func pause(with: MTRMediaPlaybackClusterPauseParams?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func pause(with: MTRMediaPlaybackClusterPauseParams?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func play(completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func play(completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func play(with: MTRMediaPlaybackClusterPlayParams?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func play(with: MTRMediaPlaybackClusterPlayParams?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func previous(completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func previous(completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func previous(with: MTRMediaPlaybackClusterPreviousParams?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func previous(with: MTRMediaPlaybackClusterPreviousParams?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func readAttributeAcceptedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeAttributeList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAttributeList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeClusterRevision(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeClusterRevision(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeCurrentState(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeCurrentState(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeDuration(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeDuration(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeFeatureMap(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFeatureMap(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeGeneratedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributePlaybackSpeed(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePlaybackSpeed(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeSampledPosition(completion: (MTRMediaPlaybackClusterPlaybackPositionStruct?, (any Error)?) -> Void)

func readAttributeSampledPosition(completionHandler: (MTRMediaPlaybackClusterPlaybackPosition?, (any Error)?) -> Void)Deprecated

func readAttributeSeekRangeEnd(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeSeekRangeEnd(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeSeekRangeStart(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeSeekRangeStart(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeStartTime(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeStartTime(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func rewind(completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func rewind(completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func rewind(with: MTRMediaPlaybackClusterRewindParams?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func rewind(with: MTRMediaPlaybackClusterRewindParams?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func seek(with: MTRMediaPlaybackClusterSeekParams, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func seek(with: MTRMediaPlaybackClusterSeekParams, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func skipBackward(with: MTRMediaPlaybackClusterSkipBackwardParams, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func skipBackward(with: MTRMediaPlaybackClusterSkipBackwardParams, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func skipForward(with: MTRMediaPlaybackClusterSkipForwardParams, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func skipForward(with: MTRMediaPlaybackClusterSkipForwardParams, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func startOver(completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func startOver(completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func startOver(with: MTRMediaPlaybackClusterStartOverParams?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func startOver(with: MTRMediaPlaybackClusterStartOverParams?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func stop(completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func stop(completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func stop(with: MTRMediaPlaybackClusterStopParams?, completion: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)

func stop(with: MTRMediaPlaybackClusterStopPlaybackParams?, completionHandler: (MTRMediaPlaybackClusterPlaybackResponseParams?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAcceptedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAttributeList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeClusterRevision(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeCurrentState(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeCurrentState(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeDuration(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeDuration(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeFeatureMap(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeGeneratedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributePlaybackSpeed(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePlaybackSpeed(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeSampledPosition(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (MTRMediaPlaybackClusterPlaybackPositionStruct?, (any Error)?) -> Void)

func subscribeAttributeSampledPosition(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (MTRMediaPlaybackClusterPlaybackPosition?, (any Error)?) -> Void)Deprecated

func subscribeAttributeSeekRangeEnd(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeSeekRangeEnd(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeSeekRangeStart(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeSeekRangeStart(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeStartTime(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeStartTime(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func activateAudioTrack(with: MTRMediaPlaybackClusterActivateAudioTrackParams, completion: MTRStatusCompletion)

Command ActivateAudioTrack

func activateTextTrack(with: MTRMediaPlaybackClusterActivateTextTrackParams, completion: MTRStatusCompletion)

Command ActivateTextTrack

func deactivateTextTrack(completion: MTRStatusCompletion)

func deactivateTextTrack(with: MTRMediaPlaybackClusterDeactivateTextTrackParams?, completion: MTRStatusCompletion)

Command DeactivateTextTrack

### Type Methods

class func readAttributeAcceptedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAcceptedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeAttributeList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAttributeList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeClusterRevision(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeCurrentState(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeCurrentState(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeDuration(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeDuration(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeFeatureMap(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeGeneratedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributePlaybackSpeed(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePlaybackSpeed(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeSampledPosition(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (MTRMediaPlaybackClusterPlaybackPosition?, (any Error)?) -> Void)Deprecated

class func readAttributeSampledPosition(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (MTRMediaPlaybackClusterPlaybackPositionStruct?, (any Error)?) -> Void)

class func readAttributeSeekRangeEnd(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeSeekRangeEnd(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeSeekRangeStart(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeSeekRangeStart(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeStartTime(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeStartTime(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

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

