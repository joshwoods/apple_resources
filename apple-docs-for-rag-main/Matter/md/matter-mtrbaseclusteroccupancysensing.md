

- Matter
-  MTRBaseClusterOccupancySensing 

Class

# MTRBaseClusterOccupancySensing

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRBaseClusterOccupancySensing
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

func readAttributeClusterRevision(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeClusterRevision(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeFeatureMap(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFeatureMap(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeGeneratedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeOccupancy(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeOccupancy(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeOccupancySensorType(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeOccupancySensorType(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeOccupancySensorTypeBitmap(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeOccupancySensorTypeBitmap(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePIROccupiedToUnoccupiedDelay(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePIRUnoccupiedToOccupiedDelay(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePIRUnoccupiedToOccupiedThreshold(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePhysicalContactOccupiedToUnoccupiedDelay(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePhysicalContactOccupiedToUnoccupiedDelay(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePhysicalContactUnoccupiedToOccupiedDelay(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePhysicalContactUnoccupiedToOccupiedDelay(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePhysicalContactUnoccupiedToOccupiedThreshold(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePhysicalContactUnoccupiedToOccupiedThreshold(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePirOccupiedToUnoccupiedDelay(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePirUnoccupiedToOccupiedDelay(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePirUnoccupiedToOccupiedThreshold(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeUltrasonicOccupiedToUnoccupiedDelay(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeUltrasonicOccupiedToUnoccupiedDelay(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeUltrasonicUnoccupiedToOccupiedDelay(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeUltrasonicUnoccupiedToOccupiedDelay(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeUltrasonicUnoccupiedToOccupiedThreshold(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeUltrasonicUnoccupiedToOccupiedThreshold(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAcceptedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAttributeList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeClusterRevision(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeFeatureMap(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeGeneratedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeOccupancy(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeOccupancy(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeOccupancySensorType(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeOccupancySensorType(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeOccupancySensorTypeBitmap(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeOccupancySensorTypeBitmap(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePIROccupiedToUnoccupiedDelay(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePIRUnoccupiedToOccupiedDelay(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePIRUnoccupiedToOccupiedThreshold(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePhysicalContactOccupiedToUnoccupiedDelay(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePhysicalContactOccupiedToUnoccupiedDelay(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePhysicalContactUnoccupiedToOccupiedDelay(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePhysicalContactUnoccupiedToOccupiedDelay(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePhysicalContactUnoccupiedToOccupiedThreshold(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePhysicalContactUnoccupiedToOccupiedThreshold(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePirOccupiedToUnoccupiedDelay(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePirUnoccupiedToOccupiedDelay(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePirUnoccupiedToOccupiedThreshold(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeUltrasonicOccupiedToUnoccupiedDelay(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeUltrasonicOccupiedToUnoccupiedDelay(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeUltrasonicUnoccupiedToOccupiedDelay(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeUltrasonicUnoccupiedToOccupiedDelay(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeUltrasonicUnoccupiedToOccupiedThreshold(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeUltrasonicUnoccupiedToOccupiedThreshold(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func writeAttributePIROccupiedToUnoccupiedDelay(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributePIROccupiedToUnoccupiedDelay(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributePIRUnoccupiedToOccupiedDelay(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributePIRUnoccupiedToOccupiedDelay(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributePIRUnoccupiedToOccupiedThreshold(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributePIRUnoccupiedToOccupiedThreshold(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributePhysicalContactOccupiedToUnoccupiedDelay(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributePhysicalContactOccupiedToUnoccupiedDelay(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributePhysicalContactOccupiedToUnoccupiedDelay(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributePhysicalContactOccupiedToUnoccupiedDelay(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributePhysicalContactUnoccupiedToOccupiedDelay(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributePhysicalContactUnoccupiedToOccupiedDelay(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributePhysicalContactUnoccupiedToOccupiedDelay(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributePhysicalContactUnoccupiedToOccupiedDelay(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributePhysicalContactUnoccupiedToOccupiedThreshold(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributePhysicalContactUnoccupiedToOccupiedThreshold(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributePhysicalContactUnoccupiedToOccupiedThreshold(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributePhysicalContactUnoccupiedToOccupiedThreshold(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributePirOccupiedToUnoccupiedDelay(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributePirOccupiedToUnoccupiedDelay(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributePirUnoccupiedToOccupiedDelay(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributePirUnoccupiedToOccupiedDelay(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributePirUnoccupiedToOccupiedThreshold(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributePirUnoccupiedToOccupiedThreshold(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeUltrasonicOccupiedToUnoccupiedDelay(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeUltrasonicOccupiedToUnoccupiedDelay(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeUltrasonicOccupiedToUnoccupiedDelay(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeUltrasonicOccupiedToUnoccupiedDelay(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeUltrasonicUnoccupiedToOccupiedDelay(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeUltrasonicUnoccupiedToOccupiedDelay(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeUltrasonicUnoccupiedToOccupiedDelay(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeUltrasonicUnoccupiedToOccupiedDelay(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeUltrasonicUnoccupiedToOccupiedThreshold(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeUltrasonicUnoccupiedToOccupiedThreshold(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeUltrasonicUnoccupiedToOccupiedThreshold(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeUltrasonicUnoccupiedToOccupiedThreshold(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func readAttributeHoldTime(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeHoldTimeLimits(completion: (MTROccupancySensingClusterHoldTimeLimitsStruct?, (any Error)?) -> Void)

func subscribeAttributeHoldTime(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeHoldTimeLimits(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (MTROccupancySensingClusterHoldTimeLimitsStruct?, (any Error)?) -> Void)

func writeAttributeHoldTime(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeHoldTime(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

### Type Methods

class func readAttributeAcceptedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAcceptedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeAttributeList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAttributeList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeClusterRevision(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeFeatureMap(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeGeneratedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeOccupancy(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeOccupancy(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeOccupancySensorType(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeOccupancySensorType(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeOccupancySensorTypeBitmap(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeOccupancySensorTypeBitmap(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePIROccupiedToUnoccupiedDelay(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePIRUnoccupiedToOccupiedDelay(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePIRUnoccupiedToOccupiedThreshold(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePhysicalContactOccupiedToUnoccupiedDelay(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePhysicalContactOccupiedToUnoccupiedDelay(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePhysicalContactUnoccupiedToOccupiedDelay(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePhysicalContactUnoccupiedToOccupiedDelay(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePhysicalContactUnoccupiedToOccupiedThreshold(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePhysicalContactUnoccupiedToOccupiedThreshold(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePirOccupiedToUnoccupiedDelay(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePirUnoccupiedToOccupiedDelay(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePirUnoccupiedToOccupiedThreshold(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeUltrasonicOccupiedToUnoccupiedDelay(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeUltrasonicOccupiedToUnoccupiedDelay(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeUltrasonicUnoccupiedToOccupiedDelay(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeUltrasonicUnoccupiedToOccupiedDelay(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeUltrasonicUnoccupiedToOccupiedThreshold(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeUltrasonicUnoccupiedToOccupiedThreshold(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeHoldTime(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeHoldTimeLimits(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (MTROccupancySensingClusterHoldTimeLimitsStruct?, (any Error)?) -> Void)

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

