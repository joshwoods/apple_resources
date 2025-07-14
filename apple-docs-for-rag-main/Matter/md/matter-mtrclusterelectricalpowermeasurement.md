

- Matter
-  MTRClusterElectricalPowerMeasurement 

Class

# MTRClusterElectricalPowerMeasurement

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class MTRClusterElectricalPowerMeasurement
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAccuracy(with: MTRReadParams?) -> [String : Any]?

func readAttributeActiveCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeActivePower(with: MTRReadParams?) -> [String : Any]?

func readAttributeApparentCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeApparentPower(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeFrequency(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeHarmonicCurrents(with: MTRReadParams?) -> [String : Any]?

func readAttributeHarmonicPhases(with: MTRReadParams?) -> [String : Any]?

func readAttributeNeutralCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfMeasurementTypes(with: MTRReadParams?) -> [String : Any]?

func readAttributePowerFactor(with: MTRReadParams?) -> [String : Any]?

func readAttributePowerMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeRMSCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeRMSPower(with: MTRReadParams?) -> [String : Any]?

func readAttributeRMSVoltage(with: MTRReadParams?) -> [String : Any]?

func readAttributeRanges(with: MTRReadParams?) -> [String : Any]?

func readAttributeReactiveCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeReactivePower(with: MTRReadParams?) -> [String : Any]?

func readAttributeVoltage(with: MTRReadParams?) -> [String : Any]?

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

