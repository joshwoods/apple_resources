

- Matter
-  MTRBaseClusterBooleanStateConfiguration 

Class

# MTRBaseClusterBooleanStateConfiguration

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class MTRBaseClusterBooleanStateConfiguration
```

## Topics

### Initializers

init?(device: MTRBaseDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func enableDisableAlarm(with: MTRBooleanStateConfigurationClusterEnableDisableAlarmParams, completion: MTRStatusCompletion)

func readAttributeAcceptedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAlarmsActive(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeAlarmsEnabled(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeAlarmsSupported(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeAlarmsSuppressed(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeAttributeList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeClusterRevision(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeCurrentSensitivityLevel(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeDefaultSensitivityLevel(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFeatureMap(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeSensorFault(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeSupportedSensitivityLevels(completion: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAlarmsActive(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeAlarmsEnabled(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeAlarmsSupported(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeAlarmsSuppressed(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeCurrentSensitivityLevel(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeDefaultSensitivityLevel(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeSensorFault(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeSupportedSensitivityLevels(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func suppressAlarm(with: MTRBooleanStateConfigurationClusterSuppressAlarmParams, completion: MTRStatusCompletion)

func writeAttributeCurrentSensitivityLevel(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeCurrentSensitivityLevel(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

### Type Methods

class func readAttributeAcceptedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeAlarmsActive(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeAlarmsEnabled(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeAlarmsSupported(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeAlarmsSuppressed(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeAttributeList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeCurrentSensitivityLevel(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeDefaultSensitivityLevel(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeSensorFault(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeSupportedSensitivityLevels(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

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

