

- Matter
-  MTRBaseClusterBallastConfiguration 

Class

# MTRBaseClusterBallastConfiguration

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRBaseClusterBallastConfiguration
```

## Topics

### Initializers

init?(device: MTRBaseDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRBaseDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeAttributeList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAttributeList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeBallastFactorAdjustment(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBallastFactorAdjustment(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeBallastStatus(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeBallastStatus(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeClusterRevision(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeClusterRevision(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeFeatureMap(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFeatureMap(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeGeneratedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeIntrinsicBalanceFactor(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeIntrinsicBallastFactor(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeLampAlarmMode(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeLampAlarmMode(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeLampBurnHours(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeLampBurnHours(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeLampBurnHoursTripPoint(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeLampBurnHoursTripPoint(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeLampManufacturer(completion: (String?, (any Error)?) -> Void)

func readAttributeLampManufacturer(completionHandler: (String?, (any Error)?) -> Void)Deprecated

func readAttributeLampQuantity(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeLampQuantity(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeLampRatedHours(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeLampRatedHours(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeLampType(completion: (String?, (any Error)?) -> Void)

func readAttributeLampType(completionHandler: (String?, (any Error)?) -> Void)Deprecated

func readAttributeMaxLevel(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeMaxLevel(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeMinLevel(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeMinLevel(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePhysicalMaxLevel(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePhysicalMaxLevel(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePhysicalMinLevel(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePhysicalMinLevel(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAcceptedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAttributeList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBallastFactorAdjustment(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBallastFactorAdjustment(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeBallastStatus(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeBallastStatus(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeClusterRevision(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeFeatureMap(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeGeneratedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeIntrinsicBalanceFactor(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeIntrinsicBallastFactor(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeLampAlarmMode(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeLampAlarmMode(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLampBurnHours(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeLampBurnHours(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLampBurnHoursTripPoint(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeLampBurnHoursTripPoint(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLampManufacturer(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)

func subscribeAttributeLampManufacturer(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLampQuantity(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeLampQuantity(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLampRatedHours(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeLampRatedHours(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLampType(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)

func subscribeAttributeLampType(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)Deprecated

func subscribeAttributeMaxLevel(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeMaxLevel(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeMinLevel(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeMinLevel(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePhysicalMaxLevel(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePhysicalMaxLevel(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePhysicalMinLevel(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePhysicalMinLevel(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func writeAttributeBallastFactorAdjustment(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeBallastFactorAdjustment(withValue: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeBallastFactorAdjustment(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeBallastFactorAdjustment(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeIntrinsicBalanceFactor(withValue: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeIntrinsicBalanceFactor(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeIntrinsicBallastFactor(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeIntrinsicBallastFactor(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeLampAlarmMode(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeLampAlarmMode(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLampAlarmMode(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeLampAlarmMode(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLampBurnHours(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeLampBurnHours(withValue: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLampBurnHours(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeLampBurnHours(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLampBurnHoursTripPoint(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeLampBurnHoursTripPoint(withValue: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLampBurnHoursTripPoint(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeLampBurnHoursTripPoint(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLampManufacturer(withValue: String, completion: MTRStatusCompletion)

func writeAttributeLampManufacturer(withValue: String, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLampManufacturer(withValue: String, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeLampManufacturer(withValue: String, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLampRatedHours(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeLampRatedHours(withValue: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLampRatedHours(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeLampRatedHours(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLampType(withValue: String, completion: MTRStatusCompletion)

func writeAttributeLampType(withValue: String, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLampType(withValue: String, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeLampType(withValue: String, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeMaxLevel(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeMaxLevel(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeMaxLevel(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeMaxLevel(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeMinLevel(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeMinLevel(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeMinLevel(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeMinLevel(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

### Type Methods

class func readAttributeAcceptedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAcceptedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeAttributeList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAttributeList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeBallastFactorAdjustment(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBallastFactorAdjustment(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeBallastStatus(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeBallastStatus(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeClusterRevision(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeFeatureMap(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeGeneratedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeIntrinsicBalanceFactor(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeIntrinsicBallastFactor(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeLampAlarmMode(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeLampAlarmMode(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeLampBurnHours(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeLampBurnHours(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeLampBurnHoursTripPoint(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeLampBurnHoursTripPoint(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeLampManufacturer(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (String?, (any Error)?) -> Void)Deprecated

class func readAttributeLampManufacturer(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (String?, (any Error)?) -> Void)

class func readAttributeLampQuantity(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeLampQuantity(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeLampRatedHours(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeLampRatedHours(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeLampType(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (String?, (any Error)?) -> Void)Deprecated

class func readAttributeLampType(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (String?, (any Error)?) -> Void)

class func readAttributeMaxLevel(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeMaxLevel(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeMinLevel(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeMinLevel(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePhysicalMaxLevel(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePhysicalMaxLevel(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePhysicalMinLevel(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePhysicalMinLevel(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

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

