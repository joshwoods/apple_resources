

- Matter
-  MTRClusterOnOffSwitchConfiguration Deprecated

Class

# MTRClusterOnOffSwitchConfiguration

iOS 16.1–18.2DeprecatediPadOS 16.1–18.2DeprecatedMac Catalyst 16.1–18.2DeprecatedmacOS 13.0–15.2DeprecatedtvOS 16.1–18.2DeprecatedvisionOS 1.0–2.2DeprecatedwatchOS 9.1–11.2Deprecated

``` source
class MTRClusterOnOffSwitchConfiguration
```

Deprecated

OnOffSwitchConfiguration is deprecated and will be removed

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeSwitchActions(with: MTRReadParams?) -> [String : Any]?

func readAttributeSwitchType(with: MTRReadParams?) -> [String : Any]?

func writeAttributeSwitchActions(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeSwitchActions(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

