

- Matter
-  MTRBaseClusterThermostat 

Class

# MTRBaseClusterThermostat

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRBaseClusterThermostat
```

## Topics

### Initializers

init?(device: MTRBaseDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRBaseDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func clearWeeklySchedule(completion: MTRStatusCompletion)

func clearWeeklySchedule(completionHandler: MTRStatusCompletion)Deprecated

func clearWeeklySchedule(with: MTRThermostatClusterClearWeeklyScheduleParams?, completion: MTRStatusCompletion)

func clearWeeklySchedule(with: MTRThermostatClusterClearWeeklyScheduleParams?, completionHandler: MTRStatusCompletion)Deprecated

func getWeeklySchedule(with: MTRThermostatClusterGetWeeklyScheduleParams, completion: (MTRThermostatClusterGetWeeklyScheduleResponseParams?, (any Error)?) -> Void)

func getWeeklySchedule(with: MTRThermostatClusterGetWeeklyScheduleParams, completionHandler: (MTRThermostatClusterGetWeeklyScheduleResponseParams?, (any Error)?) -> Void)Deprecated

func readAttributeACCapacity(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeACCapacity(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeACCapacityformat(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeACCapacityformat(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeACCoilTemperature(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeACCoilTemperature(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeACCompressorType(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeACCompressorType(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeACErrorCode(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeACErrorCode(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeACLouverPosition(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeACLouverPosition(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeACRefrigerantType(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeACRefrigerantType(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeACType(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeACType(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeAbsMaxCoolSetpointLimit(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeAbsMaxCoolSetpointLimit(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeAbsMaxHeatSetpointLimit(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeAbsMaxHeatSetpointLimit(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeAbsMinCoolSetpointLimit(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeAbsMinCoolSetpointLimit(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeAbsMinHeatSetpointLimit(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeAbsMinHeatSetpointLimit(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeAcceptedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeAttributeList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAttributeList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeClusterRevision(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeClusterRevision(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeControlSequenceOfOperation(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeControlSequenceOfOperation(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeEmergencyHeatDelta(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeEmergencyHeatDelta(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeFeatureMap(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFeatureMap(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeGeneratedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeHVACSystemTypeConfiguration(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeHVACSystemTypeConfiguration(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeLocalTemperature(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeLocalTemperature(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeLocalTemperatureCalibration(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeLocalTemperatureCalibration(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeMaxCoolSetpointLimit(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeMaxCoolSetpointLimit(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeMaxHeatSetpointLimit(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeMaxHeatSetpointLimit(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeMinCoolSetpointLimit(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeMinCoolSetpointLimit(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeMinHeatSetpointLimit(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeMinHeatSetpointLimit(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeMinSetpointDeadBand(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeMinSetpointDeadBand(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeNumberOfDailyTransitions(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNumberOfDailyTransitions(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeNumberOfWeeklyTransitions(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNumberOfWeeklyTransitions(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeOccupancy(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeOccupancy(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeOccupiedCoolingSetpoint(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeOccupiedCoolingSetpoint(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeOccupiedHeatingSetpoint(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeOccupiedHeatingSetpoint(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeOccupiedSetback(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeOccupiedSetback(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeOccupiedSetbackMax(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeOccupiedSetbackMax(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeOccupiedSetbackMin(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeOccupiedSetbackMin(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeOutdoorTemperature(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeOutdoorTemperature(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePICoolingDemand(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePICoolingDemand(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributePIHeatingDemand(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePIHeatingDemand(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeRemoteSensing(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeRemoteSensing(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeSetpointChangeAmount(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeSetpointChangeAmount(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeSetpointChangeSource(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeSetpointChangeSource(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeSetpointChangeSourceTimestamp(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeSetpointChangeSourceTimestamp(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeStartOfWeek(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeStartOfWeek(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeSystemMode(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeSystemMode(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeTemperatureSetpointHold(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeTemperatureSetpointHold(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeTemperatureSetpointHoldDuration(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeTemperatureSetpointHoldDuration(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeThermostatProgrammingOperationMode(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeThermostatProgrammingOperationMode(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeThermostatRunningMode(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeThermostatRunningMode(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeThermostatRunningState(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeThermostatRunningState(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeUnoccupiedCoolingSetpoint(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeUnoccupiedCoolingSetpoint(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeUnoccupiedHeatingSetpoint(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeUnoccupiedHeatingSetpoint(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeUnoccupiedSetback(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeUnoccupiedSetback(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeUnoccupiedSetbackMax(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeUnoccupiedSetbackMax(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeUnoccupiedSetbackMin(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeUnoccupiedSetbackMin(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func setWeeklyScheduleWith(MTRThermostatClusterSetWeeklyScheduleParams, completion: MTRStatusCompletion)

func setWeeklyScheduleWith(MTRThermostatClusterSetWeeklyScheduleParams, completionHandler: MTRStatusCompletion)Deprecated

func setpointRaiseLower(with: MTRThermostatClusterSetpointRaiseLowerParams, completion: MTRStatusCompletion)

func setpointRaiseLower(with: MTRThermostatClusterSetpointRaiseLowerParams, completionHandler: MTRStatusCompletion)Deprecated

func subscribeAttributeACCapacity(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeACCapacity(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeACCapacityformat(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeACCapacityformat(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeACCoilTemperature(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeACCoilTemperature(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeACCompressorType(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeACCompressorType(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeACErrorCode(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeACErrorCode(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeACLouverPosition(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeACLouverPosition(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeACRefrigerantType(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeACRefrigerantType(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeACType(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeACType(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAbsMaxCoolSetpointLimit(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeAbsMaxCoolSetpointLimit(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAbsMaxHeatSetpointLimit(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeAbsMaxHeatSetpointLimit(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAbsMinCoolSetpointLimit(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeAbsMinCoolSetpointLimit(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAbsMinHeatSetpointLimit(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeAbsMinHeatSetpointLimit(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAcceptedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAttributeList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeClusterRevision(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeControlSequenceOfOperation(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeControlSequenceOfOperation(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeEmergencyHeatDelta(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEmergencyHeatDelta(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeFeatureMap(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeGeneratedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeHVACSystemTypeConfiguration(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeHVACSystemTypeConfiguration(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLocalTemperature(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeLocalTemperature(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLocalTemperatureCalibration(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeLocalTemperatureCalibration(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeMaxCoolSetpointLimit(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeMaxCoolSetpointLimit(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeMaxHeatSetpointLimit(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeMaxHeatSetpointLimit(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeMinCoolSetpointLimit(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeMinCoolSetpointLimit(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeMinHeatSetpointLimit(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeMinHeatSetpointLimit(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeMinSetpointDeadBand(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeMinSetpointDeadBand(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeNumberOfDailyTransitions(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNumberOfDailyTransitions(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeNumberOfWeeklyTransitions(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNumberOfWeeklyTransitions(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeOccupancy(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeOccupancy(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeOccupiedCoolingSetpoint(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeOccupiedCoolingSetpoint(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeOccupiedHeatingSetpoint(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeOccupiedHeatingSetpoint(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeOccupiedSetback(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeOccupiedSetback(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeOccupiedSetbackMax(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeOccupiedSetbackMax(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeOccupiedSetbackMin(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeOccupiedSetbackMin(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeOutdoorTemperature(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeOutdoorTemperature(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePICoolingDemand(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePICoolingDemand(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributePIHeatingDemand(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePIHeatingDemand(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeRemoteSensing(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeRemoteSensing(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeSetpointChangeAmount(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeSetpointChangeAmount(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeSetpointChangeSource(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeSetpointChangeSource(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeSetpointChangeSourceTimestamp(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeSetpointChangeSourceTimestamp(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeStartOfWeek(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeStartOfWeek(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeSystemMode(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeSystemMode(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeTemperatureSetpointHold(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeTemperatureSetpointHold(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeTemperatureSetpointHoldDuration(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeTemperatureSetpointHoldDuration(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeThermostatProgrammingOperationMode(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeThermostatProgrammingOperationMode(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeThermostatRunningMode(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeThermostatRunningMode(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeThermostatRunningState(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeThermostatRunningState(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeUnoccupiedCoolingSetpoint(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeUnoccupiedCoolingSetpoint(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeUnoccupiedHeatingSetpoint(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeUnoccupiedHeatingSetpoint(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeUnoccupiedSetback(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeUnoccupiedSetback(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeUnoccupiedSetbackMax(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeUnoccupiedSetbackMax(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeUnoccupiedSetbackMin(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeUnoccupiedSetbackMin(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func writeAttributeACCapacity(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeACCapacity(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeACCapacity(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeACCapacity(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeACCapacityformat(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeACCapacityformat(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeACCapacityformat(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeACCapacityformat(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeACCompressorType(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeACCompressorType(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeACCompressorType(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeACCompressorType(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeACErrorCode(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeACErrorCode(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeACErrorCode(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeACErrorCode(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeACLouverPosition(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeACLouverPosition(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeACLouverPosition(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeACLouverPosition(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeACRefrigerantType(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeACRefrigerantType(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeACRefrigerantType(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeACRefrigerantType(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeACType(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeACType(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeACType(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeACType(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeControlSequenceOfOperation(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeControlSequenceOfOperation(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeControlSequenceOfOperation(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeControlSequenceOfOperation(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeEmergencyHeatDelta(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeEmergencyHeatDelta(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeEmergencyHeatDelta(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeEmergencyHeatDelta(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeHVACSystemTypeConfiguration(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeHVACSystemTypeConfiguration(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeHVACSystemTypeConfiguration(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeHVACSystemTypeConfiguration(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLocalTemperatureCalibration(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeLocalTemperatureCalibration(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLocalTemperatureCalibration(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeLocalTemperatureCalibration(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeMaxCoolSetpointLimit(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeMaxCoolSetpointLimit(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeMaxCoolSetpointLimit(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeMaxCoolSetpointLimit(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeMaxHeatSetpointLimit(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeMaxHeatSetpointLimit(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeMaxHeatSetpointLimit(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeMaxHeatSetpointLimit(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeMinCoolSetpointLimit(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeMinCoolSetpointLimit(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeMinCoolSetpointLimit(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeMinCoolSetpointLimit(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeMinHeatSetpointLimit(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeMinHeatSetpointLimit(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeMinHeatSetpointLimit(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeMinHeatSetpointLimit(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeMinSetpointDeadBand(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeMinSetpointDeadBand(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeMinSetpointDeadBand(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeMinSetpointDeadBand(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeOccupiedCoolingSetpoint(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeOccupiedCoolingSetpoint(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeOccupiedCoolingSetpoint(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeOccupiedCoolingSetpoint(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeOccupiedHeatingSetpoint(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeOccupiedHeatingSetpoint(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeOccupiedHeatingSetpoint(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeOccupiedHeatingSetpoint(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeOccupiedSetback(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeOccupiedSetback(withValue: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeOccupiedSetback(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeOccupiedSetback(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeRemoteSensing(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeRemoteSensing(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeRemoteSensing(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeRemoteSensing(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeSystemMode(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeSystemMode(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeSystemMode(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeSystemMode(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeTemperatureSetpointHold(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeTemperatureSetpointHold(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeTemperatureSetpointHold(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeTemperatureSetpointHold(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeTemperatureSetpointHoldDuration(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeTemperatureSetpointHoldDuration(withValue: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeTemperatureSetpointHoldDuration(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeTemperatureSetpointHoldDuration(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeThermostatProgrammingOperationMode(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeThermostatProgrammingOperationMode(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeThermostatProgrammingOperationMode(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeThermostatProgrammingOperationMode(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeUnoccupiedCoolingSetpoint(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeUnoccupiedCoolingSetpoint(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeUnoccupiedCoolingSetpoint(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeUnoccupiedCoolingSetpoint(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeUnoccupiedHeatingSetpoint(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeUnoccupiedHeatingSetpoint(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeUnoccupiedHeatingSetpoint(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeUnoccupiedHeatingSetpoint(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeUnoccupiedSetback(withValue: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeUnoccupiedSetback(withValue: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeUnoccupiedSetback(withValue: NSNumber?, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeUnoccupiedSetback(withValue: NSNumber?, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func atomicRequest(with: MTRThermostatClusterAtomicRequestParams, completion: (MTRThermostatClusterAtomicResponseParams?, (any Error)?) -> Void)

Command AtomicRequest

func readAttributeActivePresetHandle(completion: (Data?, (any Error)?) -> Void)

func readAttributeActiveScheduleHandle(completion: (Data?, (any Error)?) -> Void)

func readAttributeNumberOfPresets(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNumberOfScheduleTransitionPerDay(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNumberOfScheduleTransitions(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNumberOfSchedules(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributePresetTypes(completion: ([Any]?, (any Error)?) -> Void)

func readAttributePresets(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeScheduleTypes(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeSchedules(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeSetpointHoldExpiryTimestamp(completion: (NSNumber?, (any Error)?) -> Void)

func setActivePresetRequestWith(MTRThermostatClusterSetActivePresetRequestParams, completion: MTRStatusCompletion)

Command SetActivePresetRequest

func setActiveScheduleRequestWith(MTRThermostatClusterSetActiveScheduleRequestParams, completion: MTRStatusCompletion)

Command SetActiveScheduleRequest

func subscribeAttributeActivePresetHandle(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (Data?, (any Error)?) -> Void)

func subscribeAttributeActiveScheduleHandle(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (Data?, (any Error)?) -> Void)

func subscribeAttributeNumberOfPresets(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNumberOfScheduleTransitionPerDay(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNumberOfScheduleTransitions(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNumberOfSchedules(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributePresetTypes(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributePresets(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeScheduleTypes(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeSchedules(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeSetpointHoldExpiryTimestamp(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func writeAttributePresets(withValue: [Any], completion: MTRStatusCompletion)

func writeAttributePresets(withValue: [Any], params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeSchedules(withValue: [Any], completion: MTRStatusCompletion)

func writeAttributeSchedules(withValue: [Any], params: MTRWriteParams?, completion: MTRStatusCompletion)

### Type Methods

class func readAttributeACCapacity(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeACCapacity(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeACCapacityformat(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeACCapacityformat(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeACCoilTemperature(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeACCoilTemperature(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeACCompressorType(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeACCompressorType(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeACErrorCode(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeACErrorCode(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeACLouverPosition(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeACLouverPosition(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeACRefrigerantType(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeACRefrigerantType(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeACType(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeACType(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeAbsMaxCoolSetpointLimit(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeAbsMaxCoolSetpointLimit(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeAbsMaxHeatSetpointLimit(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeAbsMaxHeatSetpointLimit(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeAbsMinCoolSetpointLimit(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeAbsMinCoolSetpointLimit(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeAbsMinHeatSetpointLimit(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeAbsMinHeatSetpointLimit(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeAcceptedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAcceptedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeAttributeList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAttributeList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeClusterRevision(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeControlSequenceOfOperation(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeControlSequenceOfOperation(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEmergencyHeatDelta(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeEmergencyHeatDelta(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeFeatureMap(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeGeneratedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeHVACSystemTypeConfiguration(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeHVACSystemTypeConfiguration(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeLocalTemperature(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeLocalTemperature(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeLocalTemperatureCalibration(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeLocalTemperatureCalibration(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeMaxCoolSetpointLimit(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeMaxCoolSetpointLimit(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeMaxHeatSetpointLimit(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeMaxHeatSetpointLimit(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeMinCoolSetpointLimit(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeMinCoolSetpointLimit(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeMinHeatSetpointLimit(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeMinHeatSetpointLimit(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeMinSetpointDeadBand(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeMinSetpointDeadBand(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNumberOfDailyTransitions(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeNumberOfDailyTransitions(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNumberOfWeeklyTransitions(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeNumberOfWeeklyTransitions(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeOccupancy(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeOccupancy(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeOccupiedCoolingSetpoint(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeOccupiedCoolingSetpoint(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeOccupiedHeatingSetpoint(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeOccupiedHeatingSetpoint(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeOccupiedSetback(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeOccupiedSetback(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeOccupiedSetbackMax(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeOccupiedSetbackMax(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeOccupiedSetbackMin(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeOccupiedSetbackMin(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeOutdoorTemperature(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeOutdoorTemperature(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePICoolingDemand(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePICoolingDemand(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePIHeatingDemand(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributePIHeatingDemand(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeRemoteSensing(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeRemoteSensing(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeSetpointChangeAmount(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeSetpointChangeAmount(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeSetpointChangeSource(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeSetpointChangeSource(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeSetpointChangeSourceTimestamp(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeSetpointChangeSourceTimestamp(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeStartOfWeek(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeStartOfWeek(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeSystemMode(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeSystemMode(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeTemperatureSetpointHold(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeTemperatureSetpointHold(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeTemperatureSetpointHoldDuration(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeTemperatureSetpointHoldDuration(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeThermostatProgrammingOperationMode(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeThermostatProgrammingOperationMode(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeThermostatRunningMode(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeThermostatRunningMode(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeThermostatRunningState(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeThermostatRunningState(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeUnoccupiedCoolingSetpoint(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeUnoccupiedCoolingSetpoint(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeUnoccupiedHeatingSetpoint(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeUnoccupiedHeatingSetpoint(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeUnoccupiedSetback(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeUnoccupiedSetback(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeUnoccupiedSetbackMax(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeUnoccupiedSetbackMax(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeUnoccupiedSetbackMin(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeUnoccupiedSetbackMin(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeActivePresetHandle(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (Data?, (any Error)?) -> Void)

class func readAttributeActiveScheduleHandle(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (Data?, (any Error)?) -> Void)

class func readAttributeNumberOfPresets(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNumberOfScheduleTransitionPerDay(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNumberOfScheduleTransitions(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNumberOfSchedules(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributePresetTypes(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributePresets(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeScheduleTypes(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeSchedules(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeSetpointHoldExpiryTimestamp(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

## Relationships

### Inherits From

- MTRGenericBaseCluster

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

