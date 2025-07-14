

- Matter
-  MTRBaseClusterFanControl 

Class

# MTRBaseClusterFanControl

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRBaseClusterFanControl
```

## Topics

### Initializers

init?(device: MTRBaseDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRBaseDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeAirflowDirection(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeAttributeList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAttributeList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeClusterRevision(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeClusterRevision(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeFanMode(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFanMode(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeFanModeSequence(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFanModeSequence(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeFeatureMap(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFeatureMap(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeGeneratedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributePercentCurrent(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePercentCurrent(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePercentSetting(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePercentSetting(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeRockSetting(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeRockSetting(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeRockSupport(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeRockSupport(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeSpeedCurrent(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeSpeedCurrent(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeSpeedMax(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeSpeedMax(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeSpeedSetting(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeSpeedSetting(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeWindSetting(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeWindSetting(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeWindSupport(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeWindSupport(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func step(with: MTRFanControlClusterStepParams, completion: MTRStatusCompletion)

func subscribeAttributeAcceptedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAirflowDirection(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeClusterRevision(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeFanMode(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFanMode(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeFanModeSequence(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFanModeSequence(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeFeatureMap(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeGeneratedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributePercentCurrent(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePercentCurrent(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePercentSetting(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePercentSetting(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeRockSetting(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeRockSetting(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeRockSupport(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeRockSupport(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeSpeedCurrent(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeSpeedCurrent(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeSpeedMax(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeSpeedMax(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeSpeedSetting(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeSpeedSetting(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeWindSetting(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeWindSetting(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeWindSupport(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeWindSupport(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func writeAttributeAirflowDirection(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeAirflowDirection(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeFanMode(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeFanMode(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeFanMode(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeFanMode(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeFanModeSequence(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeFanModeSequence(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeFanModeSequence(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeFanModeSequence(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributePercentSetting(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributePercentSetting(withValue: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributePercentSetting(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributePercentSetting(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeRockSetting(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeRockSetting(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeRockSetting(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeRockSetting(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeSpeedSetting(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeSpeedSetting(withValue: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeSpeedSetting(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeSpeedSetting(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeWindSetting(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeWindSetting(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeWindSetting(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeWindSetting(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

### Type Methods

class func readAttributeAcceptedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAcceptedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeAirflowDirection(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeAttributeList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAttributeList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeClusterRevision(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFanMode(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeFanMode(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFanModeSequence(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeFanModeSequence(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeFeatureMap(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeGeneratedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributePercentCurrent(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePercentCurrent(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePercentSetting(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePercentSetting(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeRockSetting(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeRockSetting(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeRockSupport(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeRockSupport(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeSpeedCurrent(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeSpeedCurrent(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeSpeedMax(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeSpeedMax(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeSpeedSetting(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeSpeedSetting(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeWindSetting(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeWindSetting(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeWindSupport(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeWindSupport(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

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

