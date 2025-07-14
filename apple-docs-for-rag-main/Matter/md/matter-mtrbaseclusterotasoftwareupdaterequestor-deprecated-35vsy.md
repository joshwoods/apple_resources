

- Matter
-  MTRBaseClusterOtaSoftwareUpdateRequestor Deprecated

Class

# MTRBaseClusterOtaSoftwareUpdateRequestor

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
class MTRBaseClusterOtaSoftwareUpdateRequestor
```

Deprecated

Please use MTRBaseClusterOTASoftwareUpdateRequestor

## Topics

### Initializers

init?(device: MTRBaseDevice, endpoint: UInt16, queue: dispatch_queue_t)

### Instance Methods

func announceOtaProvider(with: MTROtaSoftwareUpdateRequestorClusterAnnounceOtaProviderParams, completionHandler: MTRStatusCompletion)

func readAttributeAcceptedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)

func readAttributeAttributeList(completionHandler: ([Any]?, (any Error)?) -> Void)

func readAttributeClusterRevision(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeDefaultOtaProviders(with: MTRReadParams?, completionHandler: ([Any]?, (any Error)?) -> Void)

func readAttributeFeatureMap(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)

func readAttributeUpdatePossible(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeUpdateState(completionHandler: (NSNumber?, (any Error)?) -> Void)

func readAttributeUpdateStateProgress(completionHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeDefaultOtaProviders(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeUpdatePossible(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeUpdateState(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeUpdateStateProgress(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func writeAttributeDefaultOtaProviders(withValue: [Any], completionHandler: MTRStatusCompletion)

func writeAttributeDefaultOtaProviders(withValue: [Any], params: MTRWriteParams?, completionHandler: MTRStatusCompletion)

### Type Methods

class func readAttributeAcceptedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)

class func readAttributeAttributeList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeDefaultOtaProviders(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)

class func readAttributeUpdatePossible(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeUpdateState(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

class func readAttributeUpdateStateProgress(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)

## Relationships

### Inherits From

- MTRBaseClusterOTASoftwareUpdateRequestor

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

