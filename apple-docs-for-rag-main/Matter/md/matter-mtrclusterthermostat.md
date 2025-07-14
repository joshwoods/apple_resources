

- Matter
-  MTRClusterThermostat 

Class

# MTRClusterThermostat

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterThermostat
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func clearWeeklySchedule(with: MTRThermostatClusterClearWeeklyScheduleParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func clearWeeklySchedule(with: MTRThermostatClusterClearWeeklyScheduleParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func clearWeeklySchedule(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func clearWeeklySchedule(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func getWeeklySchedule(with: MTRThermostatClusterGetWeeklyScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRThermostatClusterGetWeeklyScheduleResponseParams?, (any Error)?) -> Void)

func getWeeklySchedule(with: MTRThermostatClusterGetWeeklyScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRThermostatClusterGetWeeklyScheduleResponseParams?, (any Error)?) -> Void)Deprecated

func readAttributeACCapacity(with: MTRReadParams?) -> [String : Any]?

func readAttributeACCapacityformat(with: MTRReadParams?) -> [String : Any]?

func readAttributeACCoilTemperature(with: MTRReadParams?) -> [String : Any]?

func readAttributeACCompressorType(with: MTRReadParams?) -> [String : Any]?

func readAttributeACErrorCode(with: MTRReadParams?) -> [String : Any]?

func readAttributeACLouverPosition(with: MTRReadParams?) -> [String : Any]?

func readAttributeACRefrigerantType(with: MTRReadParams?) -> [String : Any]?

func readAttributeACType(with: MTRReadParams?) -> [String : Any]?

func readAttributeAbsMaxCoolSetpointLimit(with: MTRReadParams?) -> [String : Any]?

func readAttributeAbsMaxHeatSetpointLimit(with: MTRReadParams?) -> [String : Any]?

func readAttributeAbsMinCoolSetpointLimit(with: MTRReadParams?) -> [String : Any]?

func readAttributeAbsMinHeatSetpointLimit(with: MTRReadParams?) -> [String : Any]?

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeControlSequenceOfOperation(with: MTRReadParams?) -> [String : Any]?

func readAttributeEmergencyHeatDelta(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeHVACSystemTypeConfiguration(with: MTRReadParams?) -> [String : Any]?

func readAttributeLocalTemperature(with: MTRReadParams?) -> [String : Any]?

func readAttributeLocalTemperatureCalibration(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxCoolSetpointLimit(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxHeatSetpointLimit(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinCoolSetpointLimit(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinHeatSetpointLimit(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinSetpointDeadBand(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfDailyTransitions(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfWeeklyTransitions(with: MTRReadParams?) -> [String : Any]?

func readAttributeOccupancy(with: MTRReadParams?) -> [String : Any]?

func readAttributeOccupiedCoolingSetpoint(with: MTRReadParams?) -> [String : Any]?

func readAttributeOccupiedHeatingSetpoint(with: MTRReadParams?) -> [String : Any]?

func readAttributeOccupiedSetback(with: MTRReadParams?) -> [String : Any]?

func readAttributeOccupiedSetbackMax(with: MTRReadParams?) -> [String : Any]?

func readAttributeOccupiedSetbackMin(with: MTRReadParams?) -> [String : Any]?

func readAttributeOutdoorTemperature(with: MTRReadParams?) -> [String : Any]?

func readAttributePICoolingDemand(with: MTRReadParams?) -> [String : Any]?

func readAttributePIHeatingDemand(with: MTRReadParams?) -> [String : Any]?

func readAttributeRemoteSensing(with: MTRReadParams?) -> [String : Any]?

func readAttributeSetpointChangeAmount(with: MTRReadParams?) -> [String : Any]?

func readAttributeSetpointChangeSource(with: MTRReadParams?) -> [String : Any]?

func readAttributeSetpointChangeSourceTimestamp(with: MTRReadParams?) -> [String : Any]?

func readAttributeStartOfWeek(with: MTRReadParams?) -> [String : Any]?

func readAttributeSystemMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeTemperatureSetpointHold(with: MTRReadParams?) -> [String : Any]?

func readAttributeTemperatureSetpointHoldDuration(with: MTRReadParams?) -> [String : Any]?

func readAttributeThermostatProgrammingOperationMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeThermostatRunningMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeThermostatRunningState(with: MTRReadParams?) -> [String : Any]?

func readAttributeUnoccupiedCoolingSetpoint(with: MTRReadParams?) -> [String : Any]?

func readAttributeUnoccupiedHeatingSetpoint(with: MTRReadParams?) -> [String : Any]?

func readAttributeUnoccupiedSetback(with: MTRReadParams?) -> [String : Any]?

func readAttributeUnoccupiedSetbackMax(with: MTRReadParams?) -> [String : Any]?

func readAttributeUnoccupiedSetbackMin(with: MTRReadParams?) -> [String : Any]?

func setWeeklyScheduleWith(MTRThermostatClusterSetWeeklyScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func setWeeklyScheduleWith(MTRThermostatClusterSetWeeklyScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func setpointRaiseLower(with: MTRThermostatClusterSetpointRaiseLowerParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func setpointRaiseLower(with: MTRThermostatClusterSetpointRaiseLowerParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeACCapacity(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeACCapacity(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeACCapacityformat(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeACCapacityformat(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeACCompressorType(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeACCompressorType(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeACErrorCode(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeACErrorCode(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeACLouverPosition(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeACLouverPosition(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeACRefrigerantType(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeACRefrigerantType(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeACType(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeACType(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeControlSequenceOfOperation(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeControlSequenceOfOperation(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeEmergencyHeatDelta(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeEmergencyHeatDelta(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeHVACSystemTypeConfiguration(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeHVACSystemTypeConfiguration(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeLocalTemperatureCalibration(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeLocalTemperatureCalibration(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeMaxCoolSetpointLimit(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeMaxCoolSetpointLimit(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeMaxHeatSetpointLimit(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeMaxHeatSetpointLimit(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeMinCoolSetpointLimit(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeMinCoolSetpointLimit(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeMinHeatSetpointLimit(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeMinHeatSetpointLimit(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeMinSetpointDeadBand(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeMinSetpointDeadBand(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeOccupiedCoolingSetpoint(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeOccupiedCoolingSetpoint(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeOccupiedHeatingSetpoint(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeOccupiedHeatingSetpoint(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeOccupiedSetback(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeOccupiedSetback(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeRemoteSensing(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeRemoteSensing(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeSystemMode(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeSystemMode(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeTemperatureSetpointHold(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeTemperatureSetpointHold(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeTemperatureSetpointHoldDuration(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeTemperatureSetpointHoldDuration(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeThermostatProgrammingOperationMode(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeThermostatProgrammingOperationMode(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeUnoccupiedCoolingSetpoint(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeUnoccupiedCoolingSetpoint(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeUnoccupiedHeatingSetpoint(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeUnoccupiedHeatingSetpoint(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeUnoccupiedSetback(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeUnoccupiedSetback(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func atomicRequest(with: MTRThermostatClusterAtomicRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRThermostatClusterAtomicResponseParams?, (any Error)?) -> Void)

func readAttributeActivePresetHandle(with: MTRReadParams?) -> [String : Any]?

func readAttributeActiveScheduleHandle(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfPresets(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfScheduleTransitionPerDay(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfScheduleTransitions(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfSchedules(with: MTRReadParams?) -> [String : Any]?

func readAttributePresetTypes(with: MTRReadParams?) -> [String : Any]?

func readAttributePresets(with: MTRReadParams?) -> [String : Any]?

func readAttributeScheduleTypes(with: MTRReadParams?) -> [String : Any]?

func readAttributeSchedules(with: MTRReadParams?) -> [String : Any]?

func readAttributeSetpointHoldExpiryTimestamp(with: MTRReadParams?) -> [String : Any]?

func setActivePresetRequestWith(MTRThermostatClusterSetActivePresetRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func setActiveScheduleRequestWith(MTRThermostatClusterSetActiveScheduleRequestParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func writeAttributePresets(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributePresets(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeSchedules(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeSchedules(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

