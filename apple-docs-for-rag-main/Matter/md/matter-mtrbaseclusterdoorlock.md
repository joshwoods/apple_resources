

- Matter
-  MTRBaseClusterDoorLock 

Class

# MTRBaseClusterDoorLock

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRBaseClusterDoorLock
```

## Topics

### Initializers

init?(device: MTRBaseDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRBaseDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func clearCredential(with: MTRDoorLockClusterClearCredentialParams, completion: MTRStatusCompletion)

func clearCredential(with: MTRDoorLockClusterClearCredentialParams, completionHandler: MTRStatusCompletion)Deprecated

func clearHolidaySchedule(with: MTRDoorLockClusterClearHolidayScheduleParams, completion: MTRStatusCompletion)

func clearHolidaySchedule(with: MTRDoorLockClusterClearHolidayScheduleParams, completionHandler: MTRStatusCompletion)Deprecated

func clearUser(with: MTRDoorLockClusterClearUserParams, completion: MTRStatusCompletion)

func clearUser(with: MTRDoorLockClusterClearUserParams, completionHandler: MTRStatusCompletion)Deprecated

func clearWeekDaySchedule(with: MTRDoorLockClusterClearWeekDayScheduleParams, completion: MTRStatusCompletion)

func clearWeekDaySchedule(with: MTRDoorLockClusterClearWeekDayScheduleParams, completionHandler: MTRStatusCompletion)Deprecated

func clearYearDaySchedule(with: MTRDoorLockClusterClearYearDayScheduleParams, completion: MTRStatusCompletion)

func clearYearDaySchedule(with: MTRDoorLockClusterClearYearDayScheduleParams, completionHandler: MTRStatusCompletion)Deprecated

func getCredentialStatus(with: MTRDoorLockClusterGetCredentialStatusParams, completion: (MTRDoorLockClusterGetCredentialStatusResponseParams?, (any Error)?) -> Void)

func getCredentialStatus(with: MTRDoorLockClusterGetCredentialStatusParams, completionHandler: (MTRDoorLockClusterGetCredentialStatusResponseParams?, (any Error)?) -> Void)Deprecated

func getHolidaySchedule(with: MTRDoorLockClusterGetHolidayScheduleParams, completion: (MTRDoorLockClusterGetHolidayScheduleResponseParams?, (any Error)?) -> Void)

func getHolidaySchedule(with: MTRDoorLockClusterGetHolidayScheduleParams, completionHandler: (MTRDoorLockClusterGetHolidayScheduleResponseParams?, (any Error)?) -> Void)Deprecated

func getUserWith(MTRDoorLockClusterGetUserParams, completion: (MTRDoorLockClusterGetUserResponseParams?, (any Error)?) -> Void)

func getUserWith(MTRDoorLockClusterGetUserParams, completionHandler: (MTRDoorLockClusterGetUserResponseParams?, (any Error)?) -> Void)Deprecated

func getWeekDaySchedule(with: MTRDoorLockClusterGetWeekDayScheduleParams, completion: (MTRDoorLockClusterGetWeekDayScheduleResponseParams?, (any Error)?) -> Void)

func getWeekDaySchedule(with: MTRDoorLockClusterGetWeekDayScheduleParams, completionHandler: (MTRDoorLockClusterGetWeekDayScheduleResponseParams?, (any Error)?) -> Void)Deprecated

func getYearDaySchedule(with: MTRDoorLockClusterGetYearDayScheduleParams, completion: (MTRDoorLockClusterGetYearDayScheduleResponseParams?, (any Error)?) -> Void)

func getYearDaySchedule(with: MTRDoorLockClusterGetYearDayScheduleParams, completionHandler: (MTRDoorLockClusterGetYearDayScheduleResponseParams?, (any Error)?) -> Void)Deprecated

func lockDoor(completion: MTRStatusCompletion)

func lockDoor(with: MTRDoorLockClusterLockDoorParams?, completion: MTRStatusCompletion)

func lockDoor(with: MTRDoorLockClusterLockDoorParams?, completionHandler: MTRStatusCompletion)Deprecated

func readAttributeAcceptedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAcceptedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeActuatorEnabled(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeActuatorEnabled(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeAttributeList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAttributeList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeAutoRelockTime(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeAutoRelockTime(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeClusterRevision(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeClusterRevision(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeCredentialRulesSupport(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeCredentialRulesSupport(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeDefaultConfigurationRegister(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeDefaultConfigurationRegister(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeDoorClosedEvents(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeDoorClosedEvents(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeDoorOpenEvents(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeDoorOpenEvents(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeDoorState(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeDoorState(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeEnableInsideStatusLED(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeEnableInsideStatusLED(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeEnableLocalProgramming(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeEnableLocalProgramming(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeEnableOneTouchLocking(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeEnableOneTouchLocking(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeEnablePrivacyModeButton(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeEnablePrivacyModeButton(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeExpiringUserTimeout(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeExpiringUserTimeout(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeFeatureMap(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeFeatureMap(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeGeneratedCommandList(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeGeneratedCommandList(completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func readAttributeLEDSettings(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeLEDSettings(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeLanguage(completion: (String?, (any Error)?) -> Void)

func readAttributeLanguage(completionHandler: (String?, (any Error)?) -> Void)Deprecated

func readAttributeLocalProgrammingFeatures(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeLocalProgrammingFeatures(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeLockState(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeLockState(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeLockType(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeLockType(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeMaxPINCodeLength(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeMaxPINCodeLength(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeMaxRFIDCodeLength(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeMaxRFIDCodeLength(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeMinPINCodeLength(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeMinPINCodeLength(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeMinRFIDCodeLength(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeMinRFIDCodeLength(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeNumberOfCredentialsSupportedPerUser(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNumberOfCredentialsSupportedPerUser(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeNumberOfHolidaySchedulesSupported(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNumberOfHolidaySchedulesSupported(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeNumberOfPINUsersSupported(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNumberOfPINUsersSupported(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeNumberOfRFIDUsersSupported(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNumberOfRFIDUsersSupported(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeNumberOfTotalUsersSupported(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNumberOfTotalUsersSupported(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeNumberOfWeekDaySchedulesSupportedPerUser(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNumberOfWeekDaySchedulesSupportedPerUser(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeNumberOfYearDaySchedulesSupportedPerUser(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNumberOfYearDaySchedulesSupportedPerUser(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeOpenPeriod(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeOpenPeriod(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeOperatingMode(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeOperatingMode(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeRequirePINforRemoteOperation(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeRequirePINforRemoteOperation(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeSendPINOverTheAir(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeSendPINOverTheAir(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeSoundVolume(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeSoundVolume(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeSupportedOperatingModes(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeSupportedOperatingModes(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeUserCodeTemporaryDisableTime(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeUserCodeTemporaryDisableTime(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func readAttributeWrongCodeEntryLimit(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeWrongCodeEntryLimit(completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func setCredentialWith(MTRDoorLockClusterSetCredentialParams, completion: (MTRDoorLockClusterSetCredentialResponseParams?, (any Error)?) -> Void)

func setCredentialWith(MTRDoorLockClusterSetCredentialParams, completionHandler: (MTRDoorLockClusterSetCredentialResponseParams?, (any Error)?) -> Void)Deprecated

func setHolidayScheduleWith(MTRDoorLockClusterSetHolidayScheduleParams, completion: MTRStatusCompletion)

func setHolidayScheduleWith(MTRDoorLockClusterSetHolidayScheduleParams, completionHandler: MTRStatusCompletion)Deprecated

func setUserWith(MTRDoorLockClusterSetUserParams, completion: MTRStatusCompletion)

func setUserWith(MTRDoorLockClusterSetUserParams, completionHandler: MTRStatusCompletion)Deprecated

func setWeekDayScheduleWith(MTRDoorLockClusterSetWeekDayScheduleParams, completion: MTRStatusCompletion)

func setWeekDayScheduleWith(MTRDoorLockClusterSetWeekDayScheduleParams, completionHandler: MTRStatusCompletion)Deprecated

func setYearDayScheduleWith(MTRDoorLockClusterSetYearDayScheduleParams, completion: MTRStatusCompletion)

func setYearDayScheduleWith(MTRDoorLockClusterSetYearDayScheduleParams, completionHandler: MTRStatusCompletion)Deprecated

func subscribeAttributeAcceptedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAcceptedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeActuatorEnabled(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeActuatorEnabled(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAttributeList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAttributeList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeAutoRelockTime(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeAutoRelockTime(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeClusterRevision(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeClusterRevision(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeCredentialRulesSupport(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeCredentialRulesSupport(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeDefaultConfigurationRegister(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeDefaultConfigurationRegister(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeDoorClosedEvents(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeDoorClosedEvents(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeDoorOpenEvents(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeDoorOpenEvents(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeDoorState(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeDoorState(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeEnableInsideStatusLED(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEnableInsideStatusLED(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeEnableLocalProgramming(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEnableLocalProgramming(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeEnableOneTouchLocking(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEnableOneTouchLocking(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeEnablePrivacyModeButton(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeEnablePrivacyModeButton(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeExpiringUserTimeout(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeExpiringUserTimeout(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeFeatureMap(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeFeatureMap(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeGeneratedCommandList(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeGeneratedCommandList(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLEDSettings(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeLEDSettings(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLanguage(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)

func subscribeAttributeLanguage(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (String?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLocalProgrammingFeatures(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeLocalProgrammingFeatures(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLockState(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeLockState(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeLockType(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeLockType(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeMaxPINCodeLength(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeMaxPINCodeLength(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeMaxRFIDCodeLength(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeMaxRFIDCodeLength(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeMinPINCodeLength(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeMinPINCodeLength(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeMinRFIDCodeLength(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeMinRFIDCodeLength(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeNumberOfCredentialsSupportedPerUser(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNumberOfCredentialsSupportedPerUser(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeNumberOfHolidaySchedulesSupported(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNumberOfHolidaySchedulesSupported(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeNumberOfPINUsersSupported(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNumberOfPINUsersSupported(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeNumberOfRFIDUsersSupported(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNumberOfRFIDUsersSupported(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeNumberOfTotalUsersSupported(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNumberOfTotalUsersSupported(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeNumberOfWeekDaySchedulesSupportedPerUser(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNumberOfWeekDaySchedulesSupportedPerUser(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeNumberOfYearDaySchedulesSupportedPerUser(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNumberOfYearDaySchedulesSupportedPerUser(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeOpenPeriod(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeOpenPeriod(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeOperatingMode(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeOperatingMode(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeRequirePINforRemoteOperation(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeRequirePINforRemoteOperation(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeSendPINOverTheAir(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeSendPINOverTheAir(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeSoundVolume(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeSoundVolume(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeSupportedOperatingModes(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeSupportedOperatingModes(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeUserCodeTemporaryDisableTime(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeUserCodeTemporaryDisableTime(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func subscribeAttributeWrongCodeEntryLimit(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeWrongCodeEntryLimit(withMinInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

func unlockDoor(completion: MTRStatusCompletion)

func unlockDoor(with: MTRDoorLockClusterUnlockDoorParams?, completion: MTRStatusCompletion)

func unlockDoor(with: MTRDoorLockClusterUnlockDoorParams?, completionHandler: MTRStatusCompletion)Deprecated

func unlockWithTimeout(with: MTRDoorLockClusterUnlockWithTimeoutParams, completion: MTRStatusCompletion)

func unlockWithTimeout(with: MTRDoorLockClusterUnlockWithTimeoutParams, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeAutoRelockTime(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeAutoRelockTime(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeAutoRelockTime(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeAutoRelockTime(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeDoorClosedEvents(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeDoorClosedEvents(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeDoorClosedEvents(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeDoorClosedEvents(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeDoorOpenEvents(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeDoorOpenEvents(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeDoorOpenEvents(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeDoorOpenEvents(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeEnableInsideStatusLED(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeEnableInsideStatusLED(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeEnableInsideStatusLED(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeEnableInsideStatusLED(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeEnableLocalProgramming(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeEnableLocalProgramming(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeEnableLocalProgramming(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeEnableLocalProgramming(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeEnableOneTouchLocking(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeEnableOneTouchLocking(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeEnableOneTouchLocking(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeEnableOneTouchLocking(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeEnablePrivacyModeButton(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeEnablePrivacyModeButton(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeEnablePrivacyModeButton(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeEnablePrivacyModeButton(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeExpiringUserTimeout(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeExpiringUserTimeout(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeExpiringUserTimeout(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeExpiringUserTimeout(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLEDSettings(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeLEDSettings(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLEDSettings(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeLEDSettings(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLanguage(withValue: String, completion: MTRStatusCompletion)

func writeAttributeLanguage(withValue: String, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLanguage(withValue: String, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeLanguage(withValue: String, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLocalProgrammingFeatures(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeLocalProgrammingFeatures(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeLocalProgrammingFeatures(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeLocalProgrammingFeatures(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeOpenPeriod(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeOpenPeriod(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeOpenPeriod(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeOpenPeriod(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeOperatingMode(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeOperatingMode(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeOperatingMode(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeOperatingMode(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeRequirePINforRemoteOperation(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeRequirePINforRemoteOperation(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeRequirePINforRemoteOperation(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeRequirePINforRemoteOperation(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeSendPINOverTheAir(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeSendPINOverTheAir(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeSendPINOverTheAir(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeSendPINOverTheAir(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeSoundVolume(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeSoundVolume(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeSoundVolume(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeSoundVolume(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeUserCodeTemporaryDisableTime(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeUserCodeTemporaryDisableTime(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeUserCodeTemporaryDisableTime(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeUserCodeTemporaryDisableTime(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeWrongCodeEntryLimit(withValue: NSNumber, completion: MTRStatusCompletion)

func writeAttributeWrongCodeEntryLimit(withValue: NSNumber, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeWrongCodeEntryLimit(withValue: NSNumber, params: MTRWriteParams?, completion: MTRStatusCompletion)

func writeAttributeWrongCodeEntryLimit(withValue: NSNumber, params: MTRWriteParams?, completionHandler: MTRStatusCompletion)Deprecated

func clearAliroReaderConfig(completion: MTRStatusCompletion)

func clearAliroReaderConfig(with: MTRDoorLockClusterClearAliroReaderConfigParams?, completion: MTRStatusCompletion)

Command ClearAliroReaderConfig

func readAttributeAliroBLEAdvertisingVersion(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeAliroExpeditedTransactionSupportedProtocolVersions(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeAliroGroupResolvingKey(completion: (Data?, (any Error)?) -> Void)

func readAttributeAliroReaderGroupIdentifier(completion: (Data?, (any Error)?) -> Void)

func readAttributeAliroReaderGroupSubIdentifier(completion: (Data?, (any Error)?) -> Void)

func readAttributeAliroReaderVerificationKey(completion: (Data?, (any Error)?) -> Void)

func readAttributeAliroSupportedBLEUWBProtocolVersions(completion: ([Any]?, (any Error)?) -> Void)

func readAttributeNumberOfAliroCredentialIssuerKeysSupported(completion: (NSNumber?, (any Error)?) -> Void)

func readAttributeNumberOfAliroEndpointKeysSupported(completion: (NSNumber?, (any Error)?) -> Void)

func setAliroReaderConfigWith(MTRDoorLockClusterSetAliroReaderConfigParams, completion: MTRStatusCompletion)

Command SetAliroReaderConfig

func subscribeAttributeAliroBLEAdvertisingVersion(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeAliroExpeditedTransactionSupportedProtocolVersions(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeAliroGroupResolvingKey(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (Data?, (any Error)?) -> Void)

func subscribeAttributeAliroReaderGroupIdentifier(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (Data?, (any Error)?) -> Void)

func subscribeAttributeAliroReaderGroupSubIdentifier(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (Data?, (any Error)?) -> Void)

func subscribeAttributeAliroReaderVerificationKey(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (Data?, (any Error)?) -> Void)

func subscribeAttributeAliroSupportedBLEUWBProtocolVersions(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: ([Any]?, (any Error)?) -> Void)

func subscribeAttributeNumberOfAliroCredentialIssuerKeysSupported(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func subscribeAttributeNumberOfAliroEndpointKeysSupported(with: MTRSubscribeParams, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, reportHandler: (NSNumber?, (any Error)?) -> Void)

func unboltDoor(completion: MTRStatusCompletion)

func unboltDoor(with: MTRDoorLockClusterUnboltDoorParams?, completion: MTRStatusCompletion)

Command UnboltDoor

### Type Methods

class func readAttributeAcceptedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAcceptedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeActuatorEnabled(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeActuatorEnabled(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeAttributeList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeAttributeList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeAutoRelockTime(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeAutoRelockTime(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeClusterRevision(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeClusterRevision(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeCredentialRulesSupport(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeCredentialRulesSupport(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeDefaultConfigurationRegister(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeDefaultConfigurationRegister(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeDoorClosedEvents(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeDoorClosedEvents(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeDoorOpenEvents(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeDoorOpenEvents(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeDoorState(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeDoorState(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEnableInsideStatusLED(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeEnableInsideStatusLED(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEnableLocalProgramming(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeEnableLocalProgramming(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEnableOneTouchLocking(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeEnableOneTouchLocking(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeEnablePrivacyModeButton(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeEnablePrivacyModeButton(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeExpiringUserTimeout(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeExpiringUserTimeout(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeFeatureMap(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeFeatureMap(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeGeneratedCommandList(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: ([Any]?, (any Error)?) -> Void)Deprecated

class func readAttributeGeneratedCommandList(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeLEDSettings(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeLEDSettings(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeLanguage(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (String?, (any Error)?) -> Void)Deprecated

class func readAttributeLanguage(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (String?, (any Error)?) -> Void)

class func readAttributeLocalProgrammingFeatures(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeLocalProgrammingFeatures(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeLockState(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeLockState(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeLockType(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeLockType(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeMaxPINCodeLength(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeMaxPINCodeLength(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeMaxRFIDCodeLength(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeMaxRFIDCodeLength(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeMinPINCodeLength(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeMinPINCodeLength(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeMinRFIDCodeLength(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeMinRFIDCodeLength(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNumberOfCredentialsSupportedPerUser(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeNumberOfCredentialsSupportedPerUser(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNumberOfHolidaySchedulesSupported(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeNumberOfHolidaySchedulesSupported(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNumberOfPINUsersSupported(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeNumberOfPINUsersSupported(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNumberOfRFIDUsersSupported(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeNumberOfRFIDUsersSupported(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNumberOfTotalUsersSupported(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeNumberOfTotalUsersSupported(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNumberOfWeekDaySchedulesSupportedPerUser(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeNumberOfWeekDaySchedulesSupportedPerUser(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNumberOfYearDaySchedulesSupportedPerUser(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeNumberOfYearDaySchedulesSupportedPerUser(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeOpenPeriod(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeOpenPeriod(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeOperatingMode(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeOperatingMode(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeRequirePINforRemoteOperation(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeRequirePINforRemoteOperation(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeSendPINOverTheAir(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeSendPINOverTheAir(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeSoundVolume(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeSoundVolume(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeSupportedOperatingModes(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeSupportedOperatingModes(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeUserCodeTemporaryDisableTime(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeUserCodeTemporaryDisableTime(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeWrongCodeEntryLimit(withAttributeCache: MTRAttributeCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completionHandler: (NSNumber?, (any Error)?) -> Void)Deprecated

class func readAttributeWrongCodeEntryLimit(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeAliroBLEAdvertisingVersion(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeAliroExpeditedTransactionSupportedProtocolVersions(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeAliroGroupResolvingKey(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (Data?, (any Error)?) -> Void)

class func readAttributeAliroReaderGroupIdentifier(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (Data?, (any Error)?) -> Void)

class func readAttributeAliroReaderGroupSubIdentifier(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (Data?, (any Error)?) -> Void)

class func readAttributeAliroReaderVerificationKey(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (Data?, (any Error)?) -> Void)

class func readAttributeAliroSupportedBLEUWBProtocolVersions(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: ([Any]?, (any Error)?) -> Void)

class func readAttributeNumberOfAliroCredentialIssuerKeysSupported(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

class func readAttributeNumberOfAliroEndpointKeysSupported(withClusterStateCache: MTRClusterStateCacheContainer, endpoint: NSNumber, queue: dispatch_queue_t, completion: (NSNumber?, (any Error)?) -> Void)

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

