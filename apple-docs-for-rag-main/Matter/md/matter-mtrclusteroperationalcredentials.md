

- Matter
-  MTRClusterOperationalCredentials 

Class

# MTRClusterOperationalCredentials

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterOperationalCredentials
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func addNOC(with: MTROperationalCredentialsClusterAddNOCParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROperationalCredentialsClusterNOCResponseParams?, (any Error)?) -> Void)

func addNOC(with: MTROperationalCredentialsClusterAddNOCParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTROperationalCredentialsClusterNOCResponseParams?, (any Error)?) -> Void)Deprecated

func addTrustedRootCertificate(with: MTROperationalCredentialsClusterAddTrustedRootCertificateParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func addTrustedRootCertificate(with: MTROperationalCredentialsClusterAddTrustedRootCertificateParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func attestationRequest(with: MTROperationalCredentialsClusterAttestationRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROperationalCredentialsClusterAttestationResponseParams?, (any Error)?) -> Void)

func attestationRequest(with: MTROperationalCredentialsClusterAttestationRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTROperationalCredentialsClusterAttestationResponseParams?, (any Error)?) -> Void)Deprecated

func certificateChainRequest(with: MTROperationalCredentialsClusterCertificateChainRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROperationalCredentialsClusterCertificateChainResponseParams?, (any Error)?) -> Void)

func certificateChainRequest(with: MTROperationalCredentialsClusterCertificateChainRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTROperationalCredentialsClusterCertificateChainResponseParams?, (any Error)?) -> Void)Deprecated

func csrRequest(with: MTROperationalCredentialsClusterCSRRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROperationalCredentialsClusterCSRResponseParams?, (any Error)?) -> Void)

func csrRequest(with: MTROperationalCredentialsClusterCSRRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTROperationalCredentialsClusterCSRResponseParams?, (any Error)?) -> Void)Deprecated

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCommissionedFabrics(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentFabricIndex(with: MTRReadParams?) -> [String : Any]?

func readAttributeFabrics(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeNOCs(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupportedFabrics(with: MTRReadParams?) -> [String : Any]?

func readAttributeTrustedRootCertificates(with: MTRReadParams?) -> [String : Any]?

func removeFabric(with: MTROperationalCredentialsClusterRemoveFabricParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROperationalCredentialsClusterNOCResponseParams?, (any Error)?) -> Void)

func removeFabric(with: MTROperationalCredentialsClusterRemoveFabricParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTROperationalCredentialsClusterNOCResponseParams?, (any Error)?) -> Void)Deprecated

func updateFabricLabel(with: MTROperationalCredentialsClusterUpdateFabricLabelParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROperationalCredentialsClusterNOCResponseParams?, (any Error)?) -> Void)

func updateFabricLabel(with: MTROperationalCredentialsClusterUpdateFabricLabelParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTROperationalCredentialsClusterNOCResponseParams?, (any Error)?) -> Void)Deprecated

func updateNOC(with: MTROperationalCredentialsClusterUpdateNOCParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTROperationalCredentialsClusterNOCResponseParams?, (any Error)?) -> Void)

func updateNOC(with: MTROperationalCredentialsClusterUpdateNOCParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTROperationalCredentialsClusterNOCResponseParams?, (any Error)?) -> Void)Deprecated

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

