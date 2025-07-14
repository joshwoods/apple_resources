

- Matter
-  MTRClusterOccupancySensing 

Class

# MTRClusterOccupancySensing

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterOccupancySensing
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeOccupancy(with: MTRReadParams?) -> [String : Any]?

func readAttributeOccupancySensorType(with: MTRReadParams?) -> [String : Any]?

func readAttributeOccupancySensorTypeBitmap(with: MTRReadParams?) -> [String : Any]?

func readAttributePIROccupiedToUnoccupiedDelay(with: MTRReadParams?) -> [String : Any]?

func readAttributePIRUnoccupiedToOccupiedDelay(with: MTRReadParams?) -> [String : Any]?

func readAttributePIRUnoccupiedToOccupiedThreshold(with: MTRReadParams?) -> [String : Any]?

func readAttributePhysicalContactOccupiedToUnoccupiedDelay(with: MTRReadParams?) -> [String : Any]?

func readAttributePhysicalContactUnoccupiedToOccupiedDelay(with: MTRReadParams?) -> [String : Any]?

func readAttributePhysicalContactUnoccupiedToOccupiedThreshold(with: MTRReadParams?) -> [String : Any]?

func readAttributePirOccupiedToUnoccupiedDelay(with: MTRReadParams?) -> [String : Any]Deprecated

func readAttributePirUnoccupiedToOccupiedDelay(with: MTRReadParams?) -> [String : Any]Deprecated

func readAttributePirUnoccupiedToOccupiedThreshold(with: MTRReadParams?) -> [String : Any]Deprecated

func readAttributeUltrasonicOccupiedToUnoccupiedDelay(with: MTRReadParams?) -> [String : Any]?

func readAttributeUltrasonicUnoccupiedToOccupiedDelay(with: MTRReadParams?) -> [String : Any]?

func readAttributeUltrasonicUnoccupiedToOccupiedThreshold(with: MTRReadParams?) -> [String : Any]?

func writeAttributePIROccupiedToUnoccupiedDelay(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributePIROccupiedToUnoccupiedDelay(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributePIRUnoccupiedToOccupiedDelay(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributePIRUnoccupiedToOccupiedDelay(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributePIRUnoccupiedToOccupiedThreshold(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributePIRUnoccupiedToOccupiedThreshold(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributePhysicalContactOccupiedToUnoccupiedDelay(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributePhysicalContactOccupiedToUnoccupiedDelay(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributePhysicalContactUnoccupiedToOccupiedDelay(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributePhysicalContactUnoccupiedToOccupiedDelay(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributePhysicalContactUnoccupiedToOccupiedThreshold(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributePhysicalContactUnoccupiedToOccupiedThreshold(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributePirOccupiedToUnoccupiedDelay(withValue: [String : Any], expectedValueInterval: NSNumber)Deprecated

func writeAttributePirOccupiedToUnoccupiedDelay(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)Deprecated

func writeAttributePirUnoccupiedToOccupiedDelay(withValue: [String : Any], expectedValueInterval: NSNumber)Deprecated

func writeAttributePirUnoccupiedToOccupiedDelay(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)Deprecated

func writeAttributePirUnoccupiedToOccupiedThreshold(withValue: [String : Any], expectedValueInterval: NSNumber)Deprecated

func writeAttributePirUnoccupiedToOccupiedThreshold(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)Deprecated

func writeAttributeUltrasonicOccupiedToUnoccupiedDelay(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeUltrasonicOccupiedToUnoccupiedDelay(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeUltrasonicUnoccupiedToOccupiedDelay(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeUltrasonicUnoccupiedToOccupiedDelay(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeUltrasonicUnoccupiedToOccupiedThreshold(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeUltrasonicUnoccupiedToOccupiedThreshold(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func readAttributeHoldTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeHoldTimeLimits(with: MTRReadParams?) -> [String : Any]?

func writeAttributeHoldTime(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeHoldTime(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

