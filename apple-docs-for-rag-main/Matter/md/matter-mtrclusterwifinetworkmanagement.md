

- Matter
-  MTRClusterWiFiNetworkManagement 

Class

# MTRClusterWiFiNetworkManagement

Cluster Wi-Fi Network Management Functionality to retrieve operational information about a managed Wi-Fi network.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRClusterWiFiNetworkManagement
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

For all instance methods that take a completion (i.e. command invocations), the completion will be called on the provided queue.

### Instance Methods

func networkPassphraseRequest(with: MTRWiFiNetworkManagementClusterNetworkPassphraseRequestParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRWiFiNetworkManagementClusterNetworkPassphraseResponseParams?, (any Error)?) -> Void)

func networkPassphraseRequest(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRWiFiNetworkManagementClusterNetworkPassphraseResponseParams?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributePassphraseSurrogate(with: MTRReadParams?) -> [String : Any]?

func readAttributeSSID(with: MTRReadParams?) -> [String : Any]?

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

