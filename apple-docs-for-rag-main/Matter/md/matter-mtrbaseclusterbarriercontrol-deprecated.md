

- Matter
-  MTRBaseClusterBarrierControl Deprecated

Class

# MTRBaseClusterBarrierControl

iOS 16.1–18.2DeprecatediPadOS 16.1–18.2DeprecatedMac Catalyst 16.1–18.2DeprecatedmacOS 13.0–15.2DeprecatedtvOS 16.1–18.2DeprecatedvisionOS 1.0–2.2DeprecatedwatchOS 9.1–11.2Deprecated

``` source
class MTRBaseClusterBarrierControl
```

Deprecated

BarrierControl is deprecated and will be removed

## Topics

### Initializers

init?(device: MTRBaseDevice, endpoint: UInt16, queue: dispatch_queue_t)

init?(device: MTRBaseDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func barrierControlGoToPercent(with: MTRBarrierControlClusterBarrierControlGoToPercentParams, completion: MTRStatusCompletion)

func barrierControlGoToPercent(with: MTRBarrierControlClusterBarrierControlGoToPercentParams, completionHandler: MTRStatusCompletion)

func barrierControlStop(completion: MTRStatusCompletion)

func barrierControlStop(completionHandler: MTRStatusCompletion)

func barrierControlStop(with: MTRBarrierControlClusterBarrierControlStopParams?, completion: MTRStatusCompletion)

func barrierControlStop(with: MTRBarrierControlClusterBarrierControlStopParams?, completionHandler: MTRStatusCompletion)

func readAttributeAcceptedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)

func readAttributeAttributeList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAttributeList(completionHandler: ([Any]?, (any Error)?) -> Void)

func readAttributeBarrierCapabilities(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierCapabilities(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierCloseEvents(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierCloseEvents(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierClosePeriod(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierClosePeriod(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierCommandCloseEvents(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierCommandCloseEvents(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierCommandOpenEvents(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierCommandOpenEvents(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierMovingState(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierMovingState(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierOpenEvents(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierOpenEvents(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierOpenPeriod(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierOpenPeriod(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierPosition(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierPosition(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierSafetyStatus(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBarrierSafetyStatus(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeClusterRevision(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeClusterRevision(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeFeatureMap(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFeatureMap(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeBarrierCapabilities(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierCapabilities(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierCloseEvents(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierCloseEvents(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierClosePeriod(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierClosePeriod(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierCommandCloseEvents(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierCommandCloseEvents(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierCommandOpenEvents(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierCommandOpenEvents(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierMovingState(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierMovingState(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierOpenEvents(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierOpenEvents(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierOpenPeriod(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierOpenPeriod(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierPosition(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierPosition(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierSafetyStatus(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBarrierSafetyStatus(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func writeAttributeBarrierCloseEvents(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeBarrierCloseEvents(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeBarrierCloseEvents(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeBarrierCloseEvents(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeBarrierClosePeriod(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeBarrierClosePeriod(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeBarrierClosePeriod(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeBarrierClosePeriod(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeBarrierCommandCloseEvents(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeBarrierCommandCloseEvents(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeBarrierCommandCloseEvents(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeBarrierCommandCloseEvents(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeBarrierCommandOpenEvents(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeBarrierCommandOpenEvents(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeBarrierCommandOpenEvents(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeBarrierCommandOpenEvents(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeBarrierOpenEvents(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeBarrierOpenEvents(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeBarrierOpenEvents(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeBarrierOpenEvents(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

func writeAttributeBarrierOpenPeriod(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeBarrierOpenPeriod(withValue: NSNumber, completionHandler: MTRStatusCompletion)

func writeAttributeBarrierOpenPeriod(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeBarrierOpenPeriod(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

### Type Methods

class func readAttributeAcceptedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)

class func readAttributeAcceptedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeAttributeList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)

class func readAttributeAttributeList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeBarrierCapabilities(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierCapabilities(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierCloseEvents(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierCloseEvents(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierClosePeriod(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierClosePeriod(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierCommandCloseEvents(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierCommandCloseEvents(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierCommandOpenEvents(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierCommandOpenEvents(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierMovingState(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierMovingState(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierOpenEvents(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierOpenEvents(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierOpenPeriod(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierOpenPeriod(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierPosition(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierPosition(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierSafetyStatus(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBarrierSafetyStatus(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

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

