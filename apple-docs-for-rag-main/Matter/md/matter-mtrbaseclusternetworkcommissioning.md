

- Matter
-  MTRBaseClusterNetworkCommissioning 

Class

# MTRBaseClusterNetworkCommissioning

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRBaseClusterNetworkCommissioning
```

## Topics

### Initializers

init?(device: MTRBaseDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRBaseDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func addOrUpdateThreadNetwork(with: MTRNetworkCommissioningClusterAddOrUpdateThreadNetworkParams, completion: (MTRNetworkCommissioningClusterNetworkConfigResponseParams?, (any Error)?) -> Void)

func addOrUpdateThreadNetwork(with: MTRNetworkCommissioningClusterAddOrUpdateThreadNetworkParams, completionHandler: (MTRNetworkCommissioningClusterNetworkConfigResponseParams?, (any Error)?) -> Void)Deprecated

func addOrUpdateWiFiNetwork(with: MTRNetworkCommissioningClusterAddOrUpdateWiFiNetworkParams, completion: (MTRNetworkCommissioningClusterNetworkConfigResponseParams?, (any Error)?) -> Void)

func addOrUpdateWiFiNetwork(with: MTRNetworkCommissioningClusterAddOrUpdateWiFiNetworkParams, completionHandler: (MTRNetworkCommissioningClusterNetworkConfigResponseParams?, (any Error)?) -> Void)Deprecated

func connectNetwork(with: MTRNetworkCommissioningClusterConnectNetworkParams, completion: (MTRNetworkCommissioningClusterConnectNetworkResponseParams?, (any Error)?) -> Void)

func connectNetwork(with: MTRNetworkCommissioningClusterConnectNetworkParams, completionHandler: (MTRNetworkCommissioningClusterConnectNetworkResponseParams?, (any Error)?) -> Void)Deprecated

func readAttributeAcceptedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeAttributeList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAttributeList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeClusterRevision(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeClusterRevision(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeConnectMaxTimeSeconds(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeConnectMaxTimeSeconds(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeFeatureMap(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFeatureMap(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeGeneratedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeInterfaceEnabled(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeInterfaceEnabled(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeLastConnectErrorValue(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeLastConnectErrorValue(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeLastNetworkID(completion: (Data?, (any Error)?) -> Void)

func readAttributeLastNetworkID(completionHandler: (Data?, (any Error)?) -> Void)Deprecated

func readAttributeLastNetworkingStatus(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeLastNetworkingStatus(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeMaxNetworks(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeMaxNetworks(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeNetworks(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeNetworks(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeScanMaxTimeSeconds(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeScanMaxTimeSeconds(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func removeNetwork(with: MTRNetworkCommissioningClusterRemoveNetworkParams, completion: (MTRNetworkCommissioningClusterNetworkConfigResponseParams?, (any Error)?) -> Void)

func removeNetwork(with: MTRNetworkCommissioningClusterRemoveNetworkParams, completionHandler: (MTRNetworkCommissioningClusterNetworkConfigResponseParams?, (any Error)?) -> Void)Deprecated

func reorderNetwork(with: MTRNetworkCommissioningClusterReorderNetworkParams, completion: (MTRNetworkCommissioningClusterNetworkConfigResponseParams?, (any Error)?) -> Void)

func reorderNetwork(with: MTRNetworkCommissioningClusterReorderNetworkParams, completionHandler: (MTRNetworkCommissioningClusterNetworkConfigResponseParams?, (any Error)?) -> Void)Deprecated

func scanNetworks(completion: (MTRNetworkCommissioningClusterScanNetworksResponseParams?, (any Error)?) -> Void)

func scanNetworks(with: MTRNetworkCommissioningClusterScanNetworksParams?, completion: (MTRNetworkCommissioningClusterScanNetworksResponseParams?, (any Error)?) -> Void)

func scanNetworks(with: MTRNetworkCommissioningClusterScanNetworksParams?, completionHandler: (MTRNetworkCommissioningClusterScanNetworksResponseParams?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAcceptedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAttributeList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeClusterRevision(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeConnectMaxTimeSeconds(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeConnectMaxTimeSeconds(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeFeatureMap(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeGeneratedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeInterfaceEnabled(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeInterfaceEnabled(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLastConnectErrorValue(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeLastConnectErrorValue(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLastNetworkID(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (Data?, (any Error)?) -> Void)

func subscribeAttributeLastNetworkID(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (Data?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLastNetworkingStatus(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeLastNetworkingStatus(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeMaxNetworks(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeMaxNetworks(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeNetworks(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeNetworks(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeScanMaxTimeSeconds(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeScanMaxTimeSeconds(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func writeAttributeInterfaceEnabled(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeInterfaceEnabled(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeInterfaceEnabled(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeInterfaceEnabled(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func readAttributeSupportedThreadFeatures(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeSupportedWiFiBands(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeThreadVersion(completion: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeSupportedThreadFeatures(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeSupportedWiFiBands(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeThreadVersion(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

### Type Methods

class func readAttributeAcceptedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAcceptedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeAttributeList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAttributeList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeClusterRevision(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeConnectMaxTimeSeconds(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeConnectMaxTimeSeconds(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeFeatureMap(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeGeneratedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeInterfaceEnabled(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeInterfaceEnabled(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeLastConnectErrorValue(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeLastConnectErrorValue(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeLastNetworkID(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (Data?, (any Error)?) -> Void)Deprecated

class func readAttributeLastNetworkID(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (Data?, (any Error)?) -> Void)

class func readAttributeLastNetworkingStatus(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeLastNetworkingStatus(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeMaxNetworks(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeMaxNetworks(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNetworks(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeNetworks(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeScanMaxTimeSeconds(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeScanMaxTimeSeconds(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeSupportedThreadFeatures(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeSupportedWiFiBands(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeThreadVersion(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

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

