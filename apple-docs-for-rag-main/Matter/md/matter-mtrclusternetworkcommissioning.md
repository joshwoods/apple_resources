

- Matter
-  MTRClusterNetworkCommissioning 

Class

# MTRClusterNetworkCommissioning

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterNetworkCommissioning
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func addOrUpdateThreadNetwork(with: MTRNetworkCommissioningClusterAddOrUpdateThreadNetworkParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRNetworkCommissioningClusterNetworkConfigResponseParams?, (any Error)?) -> Void)

func addOrUpdateThreadNetwork(with: MTRNetworkCommissioningClusterAddOrUpdateThreadNetworkParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRNetworkCommissioningClusterNetworkConfigResponseParams?, (any Error)?) -> Void)Deprecated

func addOrUpdateWiFiNetwork(with: MTRNetworkCommissioningClusterAddOrUpdateWiFiNetworkParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRNetworkCommissioningClusterNetworkConfigResponseParams?, (any Error)?) -> Void)

func addOrUpdateWiFiNetwork(with: MTRNetworkCommissioningClusterAddOrUpdateWiFiNetworkParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRNetworkCommissioningClusterNetworkConfigResponseParams?, (any Error)?) -> Void)Deprecated

func connectNetwork(with: MTRNetworkCommissioningClusterConnectNetworkParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRNetworkCommissioningClusterConnectNetworkResponseParams?, (any Error)?) -> Void)

func connectNetwork(with: MTRNetworkCommissioningClusterConnectNetworkParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRNetworkCommissioningClusterConnectNetworkResponseParams?, (any Error)?) -> Void)Deprecated

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeConnectMaxTimeSeconds(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeInterfaceEnabled(with: MTRReadParams?) -> [String : Any]?

func readAttributeLastConnectErrorValue(with: MTRReadParams?) -> [String : Any]?

func readAttributeLastNetworkID(with: MTRReadParams?) -> [String : Any]?

func readAttributeLastNetworkingStatus(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxNetworks(with: MTRReadParams?) -> [String : Any]?

func readAttributeNetworks(with: MTRReadParams?) -> [String : Any]?

func readAttributeScanMaxTimeSeconds(with: MTRReadParams?) -> [String : Any]?

func removeNetwork(with: MTRNetworkCommissioningClusterRemoveNetworkParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRNetworkCommissioningClusterNetworkConfigResponseParams?, (any Error)?) -> Void)

func removeNetwork(with: MTRNetworkCommissioningClusterRemoveNetworkParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRNetworkCommissioningClusterNetworkConfigResponseParams?, (any Error)?) -> Void)Deprecated

func reorderNetwork(with: MTRNetworkCommissioningClusterReorderNetworkParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRNetworkCommissioningClusterNetworkConfigResponseParams?, (any Error)?) -> Void)

func reorderNetwork(with: MTRNetworkCommissioningClusterReorderNetworkParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRNetworkCommissioningClusterNetworkConfigResponseParams?, (any Error)?) -> Void)Deprecated

func scanNetworks(with: MTRNetworkCommissioningClusterScanNetworksParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRNetworkCommissioningClusterScanNetworksResponseParams?, (any Error)?) -> Void)

func scanNetworks(with: MTRNetworkCommissioningClusterScanNetworksParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRNetworkCommissioningClusterScanNetworksResponseParams?, (any Error)?) -> Void)Deprecated

func scanNetworks(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRNetworkCommissioningClusterScanNetworksResponseParams?, (any Error)?) -> Void)

func writeAttributeInterfaceEnabled(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeInterfaceEnabled(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func readAttributeSupportedThreadFeatures(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupportedWiFiBands(with: MTRReadParams?) -> [String : Any]?

func readAttributeThreadVersion(with: MTRReadParams?) -> [String : Any]?

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

