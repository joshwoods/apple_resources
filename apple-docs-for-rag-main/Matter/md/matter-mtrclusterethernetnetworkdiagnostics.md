

- Matter
-  MTRClusterEthernetNetworkDiagnostics 

Class

# MTRClusterEthernetNetworkDiagnostics

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterEthernetNetworkDiagnostics
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeCarrierDetect(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCollisionCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeFullDuplex(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeOverrunCount(with: MTRReadParams?) -> [String : Any]?

func readAttributePHYRate(with: MTRReadParams?) -> [String : Any]?

func readAttributePacketRxCount(with: MTRReadParams?) -> [String : Any]?

func readAttributePacketTxCount(with: MTRReadParams?) -> [String : Any]?

func readAttributeTimeSinceReset(with: MTRReadParams?) -> [String : Any]?

func readAttributeTxErrCount(with: MTRReadParams?) -> [String : Any]?

func resetCounts(with: MTREthernetNetworkDiagnosticsClusterResetCountsParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func resetCounts(with: MTREthernetNetworkDiagnosticsClusterResetCountsParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

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

