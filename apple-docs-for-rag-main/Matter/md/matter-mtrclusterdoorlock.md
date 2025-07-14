

- Matter
-  MTRClusterDoorLock 

Class

# MTRClusterDoorLock

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterDoorLock
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func clearCredential(with: MTRDoorLockClusterClearCredentialParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func clearCredential(with: MTRDoorLockClusterClearCredentialParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func clearHolidaySchedule(with: MTRDoorLockClusterClearHolidayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func clearHolidaySchedule(with: MTRDoorLockClusterClearHolidayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func clearUser(with: MTRDoorLockClusterClearUserParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func clearUser(with: MTRDoorLockClusterClearUserParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func clearWeekDaySchedule(with: MTRDoorLockClusterClearWeekDayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func clearWeekDaySchedule(with: MTRDoorLockClusterClearWeekDayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func clearYearDaySchedule(with: MTRDoorLockClusterClearYearDayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func clearYearDaySchedule(with: MTRDoorLockClusterClearYearDayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func getCredentialStatus(with: MTRDoorLockClusterGetCredentialStatusParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRDoorLockClusterGetCredentialStatusResponseParams?, (any Error)?) -> Void)

func getCredentialStatus(with: MTRDoorLockClusterGetCredentialStatusParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRDoorLockClusterGetCredentialStatusResponseParams?, (any Error)?) -> Void)Deprecated

func getHolidaySchedule(with: MTRDoorLockClusterGetHolidayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRDoorLockClusterGetHolidayScheduleResponseParams?, (any Error)?) -> Void)

func getHolidaySchedule(with: MTRDoorLockClusterGetHolidayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRDoorLockClusterGetHolidayScheduleResponseParams?, (any Error)?) -> Void)Deprecated

func getUserWith(MTRDoorLockClusterGetUserParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRDoorLockClusterGetUserResponseParams?, (any Error)?) -> Void)

func getUserWith(MTRDoorLockClusterGetUserParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRDoorLockClusterGetUserResponseParams?, (any Error)?) -> Void)Deprecated

func getWeekDaySchedule(with: MTRDoorLockClusterGetWeekDayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRDoorLockClusterGetWeekDayScheduleResponseParams?, (any Error)?) -> Void)

func getWeekDaySchedule(with: MTRDoorLockClusterGetWeekDayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRDoorLockClusterGetWeekDayScheduleResponseParams?, (any Error)?) -> Void)Deprecated

func getYearDaySchedule(with: MTRDoorLockClusterGetYearDayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRDoorLockClusterGetYearDayScheduleResponseParams?, (any Error)?) -> Void)

func getYearDaySchedule(with: MTRDoorLockClusterGetYearDayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRDoorLockClusterGetYearDayScheduleResponseParams?, (any Error)?) -> Void)Deprecated

func lockDoor(with: MTRDoorLockClusterLockDoorParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func lockDoor(with: MTRDoorLockClusterLockDoorParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func lockDoor(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeActuatorEnabled(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAutoRelockTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCredentialRulesSupport(with: MTRReadParams?) -> [String : Any]?

func readAttributeDefaultConfigurationRegister(with: MTRReadParams?) -> [String : Any]?

func readAttributeDoorClosedEvents(with: MTRReadParams?) -> [String : Any]?

func readAttributeDoorOpenEvents(with: MTRReadParams?) -> [String : Any]?

func readAttributeDoorState(with: MTRReadParams?) -> [String : Any]?

func readAttributeEnableInsideStatusLED(with: MTRReadParams?) -> [String : Any]?

func readAttributeEnableLocalProgramming(with: MTRReadParams?) -> [String : Any]?

func readAttributeEnableOneTouchLocking(with: MTRReadParams?) -> [String : Any]?

func readAttributeEnablePrivacyModeButton(with: MTRReadParams?) -> [String : Any]?

func readAttributeExpiringUserTimeout(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeLEDSettings(with: MTRReadParams?) -> [String : Any]?

func readAttributeLanguage(with: MTRReadParams?) -> [String : Any]?

func readAttributeLocalProgrammingFeatures(with: MTRReadParams?) -> [String : Any]?

func readAttributeLockState(with: MTRReadParams?) -> [String : Any]?

func readAttributeLockType(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxPINCodeLength(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxRFIDCodeLength(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinPINCodeLength(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinRFIDCodeLength(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfCredentialsSupportedPerUser(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfHolidaySchedulesSupported(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfPINUsersSupported(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfRFIDUsersSupported(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfTotalUsersSupported(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfWeekDaySchedulesSupportedPerUser(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfYearDaySchedulesSupportedPerUser(with: MTRReadParams?) -> [String : Any]?

func readAttributeOpenPeriod(with: MTRReadParams?) -> [String : Any]?

func readAttributeOperatingMode(with: MTRReadParams?) -> [String : Any]?

func readAttributeRequirePINforRemoteOperation(with: MTRReadParams?) -> [String : Any]?

func readAttributeSendPINOverTheAir(with: MTRReadParams?) -> [String : Any]?

func readAttributeSoundVolume(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupportedOperatingModes(with: MTRReadParams?) -> [String : Any]?

func readAttributeUserCodeTemporaryDisableTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeWrongCodeEntryLimit(with: MTRReadParams?) -> [String : Any]?

func setCredentialWith(MTRDoorLockClusterSetCredentialParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: (MTRDoorLockClusterSetCredentialResponseParams?, (any Error)?) -> Void)

func setCredentialWith(MTRDoorLockClusterSetCredentialParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: (MTRDoorLockClusterSetCredentialResponseParams?, (any Error)?) -> Void)Deprecated

func setHolidayScheduleWith(MTRDoorLockClusterSetHolidayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func setHolidayScheduleWith(MTRDoorLockClusterSetHolidayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func setUserWith(MTRDoorLockClusterSetUserParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func setUserWith(MTRDoorLockClusterSetUserParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func setWeekDayScheduleWith(MTRDoorLockClusterSetWeekDayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func setWeekDayScheduleWith(MTRDoorLockClusterSetWeekDayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func setYearDayScheduleWith(MTRDoorLockClusterSetYearDayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func setYearDayScheduleWith(MTRDoorLockClusterSetYearDayScheduleParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func unlockDoor(with: MTRDoorLockClusterUnlockDoorParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func unlockDoor(with: MTRDoorLockClusterUnlockDoorParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func unlockDoor(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func unlockWithTimeout(with: MTRDoorLockClusterUnlockWithTimeoutParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func unlockWithTimeout(with: MTRDoorLockClusterUnlockWithTimeoutParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completionHandler: MTRStatusCompletion)Deprecated

func writeAttributeAutoRelockTime(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeAutoRelockTime(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeDoorClosedEvents(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeDoorClosedEvents(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeDoorOpenEvents(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeDoorOpenEvents(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeEnableInsideStatusLED(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeEnableInsideStatusLED(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeEnableLocalProgramming(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeEnableLocalProgramming(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeEnableOneTouchLocking(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeEnableOneTouchLocking(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeEnablePrivacyModeButton(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeEnablePrivacyModeButton(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeExpiringUserTimeout(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeExpiringUserTimeout(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeLEDSettings(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeLEDSettings(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeLanguage(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeLanguage(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeLocalProgrammingFeatures(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeLocalProgrammingFeatures(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeOpenPeriod(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeOpenPeriod(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeOperatingMode(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeOperatingMode(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeRequirePINforRemoteOperation(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeRequirePINforRemoteOperation(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeSendPINOverTheAir(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeSendPINOverTheAir(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeSoundVolume(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeSoundVolume(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeUserCodeTemporaryDisableTime(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeUserCodeTemporaryDisableTime(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeWrongCodeEntryLimit(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeWrongCodeEntryLimit(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func clearAliroReaderConfig(with: MTRDoorLockClusterClearAliroReaderConfigParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func clearAliroReaderConfig(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func readAttributeAliroBLEAdvertisingVersion(with: MTRReadParams?) -> [String : Any]?

func readAttributeAliroExpeditedTransactionSupportedProtocolVersions(with: MTRReadParams?) -> [String : Any]?

func readAttributeAliroGroupResolvingKey(with: MTRReadParams?) -> [String : Any]?

func readAttributeAliroReaderGroupIdentifier(with: MTRReadParams?) -> [String : Any]?

func readAttributeAliroReaderGroupSubIdentifier(with: MTRReadParams?) -> [String : Any]?

func readAttributeAliroReaderVerificationKey(with: MTRReadParams?) -> [String : Any]?

func readAttributeAliroSupportedBLEUWBProtocolVersions(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfAliroCredentialIssuerKeysSupported(with: MTRReadParams?) -> [String : Any]?

func readAttributeNumberOfAliroEndpointKeysSupported(with: MTRReadParams?) -> [String : Any]?

func setAliroReaderConfigWith(MTRDoorLockClusterSetAliroReaderConfigParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func unboltDoor(with: MTRDoorLockClusterUnboltDoorParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func unboltDoor(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

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

