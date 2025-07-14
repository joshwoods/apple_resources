

- Matter
-  MTRClusterBinaryInputBasic Deprecated

Class

# MTRClusterBinaryInputBasic

iOS 16.1–18.2DeprecatediPadOS 16.1–18.2DeprecatedMac Catalyst 16.1–18.2DeprecatedmacOS 13.0–15.2DeprecatedtvOS 16.1–18.2DeprecatedvisionOS 1.0–2.2DeprecatedwatchOS 9.1–11.2Deprecated

``` source
class MTRClusterBinaryInputBasic
```

Deprecated

BinaryInputBasic is deprecated and will be removed

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeActiveText(with: MTRReadParams?) -> [String : Any]?

func readAttributeApplicationType(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeDescription(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeInactiveText(with: MTRReadParams?) -> [String : Any]?

func readAttributeOutOfService(with: MTRReadParams?) -> [String : Any]?

func readAttributePolarity(with: MTRReadParams?) -> [String : Any]?

func readAttributePresentValue(with: MTRReadParams?) -> [String : Any]?

func readAttributeReliability(with: MTRReadParams?) -> [String : Any]?

func readAttributeStatusFlags(with: MTRReadParams?) -> [String : Any]?

func writeAttributeActiveText(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeActiveText(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeDescription(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeDescription(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeInactiveText(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeInactiveText(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeOutOfService(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeOutOfService(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributePresentValue(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributePresentValue(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeReliability(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeReliability(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

