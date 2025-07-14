

- Matter
-  MTRClusterBarrierControl Deprecated

Class

# MTRClusterBarrierControl

iOS 16.1–18.2DeprecatediPadOS 16.1–18.2DeprecatedMac Catalyst 16.1–18.2DeprecatedmacOS 13.0–15.2DeprecatedtvOS 16.1–18.2DeprecatedvisionOS 1.0–2.2DeprecatedwatchOS 9.1–11.2Deprecated

``` source
class MTRClusterBarrierControl
```

Deprecated

BarrierControl is deprecated and will be removed

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func barrierControlGoToPercent(with: MTRBarrierControlClusterBarrierControlGoToPercentParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func barrierControlGoToPercent(with: MTRBarrierControlClusterBarrierControlGoToPercentParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func barrierControlStop(with: MTRBarrierControlClusterBarrierControlStopParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func barrierControlStop(with: MTRBarrierControlClusterBarrierControlStopParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func barrierControlStop(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func barrierControlStop(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeBarrierCapabilities(with: MTRReadParams?) -> [String : Any]?

func readAttributeBarrierCloseEvents(with: MTRReadParams?) -> [String : Any]?

func readAttributeBarrierClosePeriod(with: MTRReadParams?) -> [String : Any]?

func readAttributeBarrierCommandCloseEvents(with: MTRReadParams?) -> [String : Any]?

func readAttributeBarrierCommandOpenEvents(with: MTRReadParams?) -> [String : Any]?

func readAttributeBarrierMovingState(with: MTRReadParams?) -> [String : Any]?

func readAttributeBarrierOpenEvents(with: MTRReadParams?) -> [String : Any]?

func readAttributeBarrierOpenPeriod(with: MTRReadParams?) -> [String : Any]?

func readAttributeBarrierPosition(with: MTRReadParams?) -> [String : Any]?

func readAttributeBarrierSafetyStatus(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func writeAttributeBarrierCloseEvents(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeBarrierCloseEvents(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeBarrierClosePeriod(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeBarrierClosePeriod(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeBarrierCommandCloseEvents(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeBarrierCommandCloseEvents(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeBarrierCommandOpenEvents(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeBarrierCommandOpenEvents(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeBarrierOpenEvents(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeBarrierOpenEvents(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeBarrierOpenPeriod(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeBarrierOpenPeriod(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

