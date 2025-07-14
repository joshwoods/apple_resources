

- Matter
-  MTRClusterBallastConfiguration 

Class

# MTRClusterBallastConfiguration

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterBallastConfiguration
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeBallastFactorAdjustment(with: MTRReadParams?) -> [String : Any]?

func readAttributeBallastStatus(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeIntrinsicBalanceFactor(with: MTRReadParams?) -> [String : Any]Deprecated

func readAttributeIntrinsicBallastFactor(with: MTRReadParams?) -> [String : Any]?

func readAttributeLampAlarmMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeLampBurnHours(with: MTRReadParams?) -> [String : Any]?

func readAttributeLampBurnHoursTripPoint(with: MTRReadParams?) -> [String : Any]?

func readAttributeLampManufacturer(with: MTRReadParams?) -> [String : Any]?

func readAttributeLampQuantity(with: MTRReadParams?) -> [String : Any]?

func readAttributeLampRatedHours(with: MTRReadParams?) -> [String : Any]?

func readAttributeLampType(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxLevel(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinLevel(with: MTRReadParams?) -> [String : Any]?

func readAttributePhysicalMaxLevel(with: MTRReadParams?) -> [String : Any]?

func readAttributePhysicalMinLevel(with: MTRReadParams?) -> [String : Any]?

func writeAttributeBallastFactorAdjustment(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeBallastFactorAdjustment(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeIntrinsicBalanceFactor(withValue: [String : Any], expectedValueInterval: NSNumber)Deprecated

func writeAttributeIntrinsicBalanceFactor(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)Deprecated

func writeAttributeIntrinsicBallastFactor(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeIntrinsicBallastFactor(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeLampAlarmMode(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeLampAlarmMode(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeLampBurnHours(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeLampBurnHours(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeLampBurnHoursTripPoint(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeLampBurnHoursTripPoint(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeLampManufacturer(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeLampManufacturer(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeLampRatedHours(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeLampRatedHours(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeLampType(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeLampType(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeMaxLevel(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeMaxLevel(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeMinLevel(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeMinLevel(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

