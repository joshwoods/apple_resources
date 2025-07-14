

- Matter
-  MTRClusterElectricalMeasurement Deprecated

Class

# MTRClusterElectricalMeasurement

iOS 16.1–18.2DeprecatediPadOS 16.1–18.2DeprecatedMac Catalyst 16.1–18.2DeprecatedmacOS 13.0–15.2DeprecatedtvOS 16.1–18.2DeprecatedvisionOS 1.0–2.2DeprecatedwatchOS 9.1–11.2Deprecated

``` source
class MTRClusterElectricalMeasurement
```

Deprecated

ElectricalMeasurement is deprecated and will be removed

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func getProfileCommand(with: MTRElectricalMeasurementClusterGetMeasurementProfileCommandParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func getProfileCommand(with: MTRElectricalMeasurementClusterGetMeasurementProfileCommandParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func getProfileInfoCommand(with: MTRElectricalMeasurementClusterGetProfileInfoCommandParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func getProfileInfoCommand(with: MTRElectricalMeasurementClusterGetProfileInfoCommandParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func getProfileInfoCommand(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func getProfileInfoCommand(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)

func readAttributeAcActivePowerOverload(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcCurrentDivisor(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcCurrentMultiplier(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcCurrentOverload(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcFrequency(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcFrequencyDivisor(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcFrequencyMax(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcFrequencyMin(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcFrequencyMultiplier(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcOverloadAlarmsMask(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcPowerDivisor(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcPowerMultiplier(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcReactivePowerOverload(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcVoltageDivisor(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcVoltageMultiplier(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcVoltageOverload(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeActiveCurrentPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeActiveCurrentPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeActivePower(with: MTRReadParams?) -> [String : Any]?

func readAttributeActivePowerMax(with: MTRReadParams?) -> [String : Any]?

func readAttributeActivePowerMaxPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeActivePowerMaxPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeActivePowerMin(with: MTRReadParams?) -> [String : Any]?

func readAttributeActivePowerMinPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeActivePowerMinPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeActivePowerPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeActivePowerPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeApparentPower(with: MTRReadParams?) -> [String : Any]?

func readAttributeApparentPowerPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeApparentPowerPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAverageRmsOverVoltage(with: MTRReadParams?) -> [String : Any]?

func readAttributeAverageRmsOverVoltageCounterPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeAverageRmsOverVoltageCounterPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeAverageRmsUnderVoltage(with: MTRReadParams?) -> [String : Any]?

func readAttributeAverageRmsUnderVoltageCounter(with: MTRReadParams?) -> [String : Any]?

func readAttributeAverageRmsUnderVoltageCounterPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeAverageRmsUnderVoltageCounterPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeAverageRmsVoltageMeasurementPeriod(with: MTRReadParams?) -> [String : Any]?

func readAttributeAverageRmsVoltageMeasurementPeriodPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeAverageRmsVoltageMeasurementPeriodPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentOverload(with: MTRReadParams?) -> [String : Any]?

func readAttributeDcCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeDcCurrentDivisor(with: MTRReadParams?) -> [String : Any]?

func readAttributeDcCurrentMax(with: MTRReadParams?) -> [String : Any]?

func readAttributeDcCurrentMin(with: MTRReadParams?) -> [String : Any]?

func readAttributeDcCurrentMultiplier(with: MTRReadParams?) -> [String : Any]?

func readAttributeDcPower(with: MTRReadParams?) -> [String : Any]?

func readAttributeDcPowerDivisor(with: MTRReadParams?) -> [String : Any]?

func readAttributeDcPowerMax(with: MTRReadParams?) -> [String : Any]?

func readAttributeDcPowerMin(with: MTRReadParams?) -> [String : Any]?

func readAttributeDcPowerMultiplier(with: MTRReadParams?) -> [String : Any]?

func readAttributeDcVoltage(with: MTRReadParams?) -> [String : Any]?

func readAttributeDcVoltageDivisor(with: MTRReadParams?) -> [String : Any]?

func readAttributeDcVoltageMax(with: MTRReadParams?) -> [String : Any]?

func readAttributeDcVoltageMin(with: MTRReadParams?) -> [String : Any]?

func readAttributeDcVoltageMultiplier(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeHarmonicCurrentMultiplier(with: MTRReadParams?) -> [String : Any]?

func readAttributeInstantaneousActiveCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeInstantaneousLineCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeInstantaneousPower(with: MTRReadParams?) -> [String : Any]?

func readAttributeInstantaneousReactiveCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeInstantaneousVoltage(with: MTRReadParams?) -> [String : Any]?

func readAttributeLineCurrentPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeLineCurrentPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeasured11thHarmonicCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeasured1stHarmonicCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeasured3rdHarmonicCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeasured5thHarmonicCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeasured7thHarmonicCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeasured9thHarmonicCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeasuredPhase11thHarmonicCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeasuredPhase1stHarmonicCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeasuredPhase3rdHarmonicCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeasuredPhase5thHarmonicCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeasuredPhase7thHarmonicCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeasuredPhase9thHarmonicCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeasurementType(with: MTRReadParams?) -> [String : Any]?

func readAttributeNeutralCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeOverloadAlarmsMask(with: MTRReadParams?) -> [String : Any]?

func readAttributePhaseHarmonicCurrentMultiplier(with: MTRReadParams?) -> [String : Any]?

func readAttributePowerDivisor(with: MTRReadParams?) -> [String : Any]?

func readAttributePowerFactor(with: MTRReadParams?) -> [String : Any]?

func readAttributePowerFactorPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributePowerFactorPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributePowerMultiplier(with: MTRReadParams?) -> [String : Any]?

func readAttributeReactiveCurrentPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeReactiveCurrentPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeReactivePower(with: MTRReadParams?) -> [String : Any]?

func readAttributeReactivePowerPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeReactivePowerPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsCurrent(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsCurrentMax(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsCurrentMaxPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsCurrentMaxPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsCurrentMin(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsCurrentMinPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsCurrentMinPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsCurrentPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsCurrentPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsExtremeOverVoltage(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsExtremeOverVoltagePeriod(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsExtremeOverVoltagePeriodPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsExtremeOverVoltagePeriodPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsExtremeUnderVoltage(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsExtremeUnderVoltagePeriod(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsExtremeUnderVoltagePeriodPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsExtremeUnderVoltagePeriodPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltage(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltageMax(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltageMaxPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltageMaxPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltageMin(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltageMinPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltageMinPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltagePhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltagePhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltageSag(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltageSagPeriod(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltageSagPeriodPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltageSagPeriodPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltageSwell(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltageSwellPeriod(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltageSwellPeriodPhaseB(with: MTRReadParams?) -> [String : Any]?

func readAttributeRmsVoltageSwellPeriodPhaseC(with: MTRReadParams?) -> [String : Any]?

func readAttributeTotalActivePower(with: MTRReadParams?) -> [String : Any]?

func readAttributeTotalApparentPower(with: MTRReadParams?) -> [String : Any]?

func readAttributeTotalReactivePower(with: MTRReadParams?) -> [String : Any]?

func readAttributeVoltageOverload(with: MTRReadParams?) -> [String : Any]?

func writeAttributeAcOverloadAlarmsMask(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeAcOverloadAlarmsMask(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeAverageRmsUnderVoltageCounter(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeAverageRmsUnderVoltageCounter(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeAverageRmsVoltageMeasurementPeriod(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeAverageRmsVoltageMeasurementPeriod(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeOverloadAlarmsMask(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeOverloadAlarmsMask(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeRmsExtremeOverVoltagePeriod(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeRmsExtremeOverVoltagePeriod(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeRmsExtremeUnderVoltagePeriod(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeRmsExtremeUnderVoltagePeriod(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeRmsVoltageSagPeriod(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeRmsVoltageSagPeriod(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeRmsVoltageSwellPeriod(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeRmsVoltageSwellPeriod(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

