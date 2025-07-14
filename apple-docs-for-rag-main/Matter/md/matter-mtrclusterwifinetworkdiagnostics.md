

- Matter
-  MTRClusterWiFiNetworkDiagnostics 

Class

# MTRClusterWiFiNetworkDiagnostics

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterWiFiNetworkDiagnostics
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeBSSID(with: MTRReadParams?) -> [String : Any]?

func readAttributeBeaconLostCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeBeaconRxCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeBssid(with: MTRReadParams?) -> [String : Any]Deprecated

func readAttributeChannelNumber(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentMaxRate(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeOverrunCount(with: MTRReadParams?) -> [String : Any]?

func readAttributePacketMulticastRxCount(with: MTRReadParams?) -> [String : Any]?

func readAttributePacketMulticastTxCount(with: MTRReadParams?) -> [String : Any]?

func readAttributePacketUnicastRxCount(with: MTRReadParams?) -> [String : Any]?

func readAttributePacketUnicastTxCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeRSSI(with: MTRReadParams?) -> [String : Any]?

func readAttributeRssi(with: MTRReadParams?) -> [String : Any]Deprecated

func readAttributeSecurityType(with: MTRReadParams?) -> [String : Any]?

func readAttributeWiFiVersion(with: MTRReadParams?) -> [String : Any]?

func resetCounts(with: MTRWiFiNetworkDiagnosticsClusterResetCountsParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func resetCounts(with: MTRWiFiNetworkDiagnosticsClusterResetCountsParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func resetCounts(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func resetCounts(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

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

