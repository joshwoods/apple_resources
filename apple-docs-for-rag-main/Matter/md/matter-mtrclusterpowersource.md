

- Matter
-  MTRClusterPowerSource 

Class

# MTRClusterPowerSource

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterPowerSource
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeActiveBatChargeFaults(with: MTRReadParams?) -> [String : Any]?

func readAttributeActiveBatFaults(with: MTRReadParams?) -> [String : Any]?

func readAttributeActiveWiredFaults(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatANSIDesignation(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatApprovedChemistry(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatCapacity(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatChargeLevel(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatChargeState(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatChargingCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatCommonDesignation(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatFunctionalWhileCharging(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatIECDesignation(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatPercentRemaining(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatPresent(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatQuantity(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatReplaceability(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatReplacementDescription(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatReplacementNeeded(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatTimeRemaining(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatTimeToFullCharge(with: MTRReadParams?) -> [String : Any]?

func readAttributeBatVoltage(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeDescription(with: MTRReadParams?) -> [String : Any]?

func readAttributeEndpointList(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeOrder(with: MTRReadParams?) -> [String : Any]?

func readAttributeStatus(with: MTRReadParams?) -> [String : Any]?

func readAttributeWiredAssessedCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeWiredAssessedInputFrequency(with: MTRReadParams?) -> [String : Any]?

func readAttributeWiredAssessedInputVoltage(with: MTRReadParams?) -> [String : Any]?

func readAttributeWiredCurrentType(with: MTRReadParams?) -> [String : Any]?

func readAttributeWiredMaximumCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeWiredNominalVoltage(with: MTRReadParams?) -> [String : Any]?

func readAttributeWiredPresent(with: MTRReadParams?) -> [String : Any]?

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

