

- Matter
-  MTRClusterGeneralCommissioning 

Class

# MTRClusterGeneralCommissioning

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterGeneralCommissioning
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func armFailSafe(with: MTRGeneralCommissioningClusterArmFailSafeParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRGeneralCommissioningClusterArmFailSafeResponseParams?, (any Error)?) -> Void)

func armFailSafe(with: MTRGeneralCommissioningClusterArmFailSafeParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRGeneralCommissioningClusterArmFailSafeResponseParams?, (any Error)?) -> Void)Deprecated

func commissioningComplete(with: MTRGeneralCommissioningClusterCommissioningCompleteParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRGeneralCommissioningClusterCommissioningCompleteResponseParams?, (any Error)?) -> Void)

func commissioningComplete(with: MTRGeneralCommissioningClusterCommissioningCompleteParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRGeneralCommissioningClusterCommissioningCompleteResponseParams?, (any Error)?) -> Void)Deprecated

func commissioningComplete(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRGeneralCommissioningClusterCommissioningCompleteResponseParams?, (any Error)?) -> Void)

func commissioningComplete(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRGeneralCommissioningClusterCommissioningCompleteResponseParams?, (any Error)?) -> Void)Deprecated

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeBasicCommissioningInfo(with: MTRReadParams?) -> [String : Any]?

func readAttributeBreadcrumb(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeLocationCapability(with: MTRReadParams?) -> [String : Any]?

func readAttributeRegulatoryConfig(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupportsConcurrentConnection(with: MTRReadParams?) -> [String : Any]?

func setRegulatoryConfigWith(MTRGeneralCommissioningClusterSetRegulatoryConfigParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRGeneralCommissioningClusterSetRegulatoryConfigResponseParams?, (any Error)?) -> Void)

func setRegulatoryConfigWith(MTRGeneralCommissioningClusterSetRegulatoryConfigParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRGeneralCommissioningClusterSetRegulatoryConfigResponseParams?, (any Error)?) -> Void)Deprecated

func writeAttributeBreadcrumb(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeBreadcrumb(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

