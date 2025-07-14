

- Kernel
- Driver Support
-  IOPMrootDomain 

Class

# IOPMrootDomain

macOS 10.0+

``` source
class IOPMrootDomain : IOService
```

## Topics

### Instance Methods

- askChangeDown

- callPlatformFunction

- changePowerStateTo

- changePowerStateToPriv

- claimSystemBootEvent

- claimSystemShutdownEvent

- claimSystemWakeEvent

- configureReport

- configureReportGated

- copyPMSetting

- copyProperty

- copyWakeReasonString

- createPMAssertion

- getAggressiveness

- getMetaClass

- getPMAssertionLevel

- getRUN_STATE

- getSleepSupported

- powerChangeDone

- publishFeature

- publishFeature

- receivePowerNotification

- registerInterest

- registerPMSettingController

- registerPMSettingController

- releasePMAssertion

- removePublishedFeature

- requestPowerDomainState

- requestUserActive

- restartWithStackshot

- serializeProperties

- setAggressiveness

- setPMAssertionLevel

- setProperties

- setSleepSupported

- setWakeTime

- sleepSystem

- sleepSystemOptions

- start

- systemPowerEventOccurred

- systemPowerEventOccurred

- tellChangeDown

- tellChangeUp

- tellNoChangeDown

- updateReport

- updateReportGated

- wakeFromDoze

### Type Methods

+ construct

## Relationships

### Inherits From

- IOService

## See Also

### Power Management

IOACPIPlatformDevice

IOACPIPlatformExpert

IOPMPowerSource

IOPMPowerSourceList

IOPowerConnection

IOPwrController

IOACPIAddress

IOACPIAddressSpaceDescriptor

IOACPIAddressSpaceHandler

IOACPIAddressSpaceID

IOPMPowerState

acknowledgeSleepWakeNotification

gIOACPIAddressKey

gIOACPIDeviceStatusKey

gIOACPIHardwareIDKey

gIOACPIPlane

gIOACPIUniqueIDKey

