

- Kernel
- Driver Support
-  IOPowerConnection 

Class

# IOPowerConnection

macOS 10.0+

``` source
class IOPowerConnection : IOService
```

## Overview

Do not use IOPowerConnection. This class is an implementation detail defined for IOPM's management of the IORegistry IOPower plane.

Only Kernel IOKit power management should reference the IOPowerConnection class.

## Topics

### Miscellaneous

childHasRequestedPower

Return the flag that says whether the child has called requestPowerDomainState.

getAwaitingAck

Returns the awaitingAck variable.

getDesiredDomainState

Returns the desiredDomainState variable.

getPreventIdleSleepFlag

Returns the preventIdleSleepFlag variable.

getPreventSystemSleepFlag

Returns the preventSystemSleepFlag variable.

getReadyFlag

Returns the readyFlag variable.

parentCurrentPowerFlags

Returns the currentPowerFlags variable.

parentKnowsState

Returns the stateKnown variable.

setAwaitingAck

Sets the awaitingAck variable.

setChildHasRequestedPower

Set the flag that says that the child has called requestPowerDomainState.

setDesiredDomainState

Sets the desiredDomainState variable.

setParentCurrentPowerFlags

Sets the currentPowerFlags variable.

setParentKnowsState

Sets the stateKnown variable.

setPreventIdleSleepFlag

Sets the preventIdleSleepFlag variable.

setPreventSystemSleepFlag

Sets the preventSystemSleepFlag variable.

setReadyFlag

Sets the readyFlag variable.

### Instance Variables

stateKnown

requestFlag

readyFlag

preventSystemSleepFlag

preventIdleSleepFlag

desiredDomainState

currentPowerFlags

awaitingAck

### Instance Methods

- childHasRequestedPower

- getAwaitingAck

- getDesiredDomainState

- getMetaClass

- getPreventIdleSleepFlag

- getPreventSystemSleepFlag

- getReadyFlag

- parentCurrentPowerFlags

- parentKnowsState

- setAwaitingAck

- setChildHasRequestedPower

- setDesiredDomainState

- setParentCurrentPowerFlags

- setParentKnowsState

- setPreventIdleSleepFlag

- setPreventSystemSleepFlag

- setReadyFlag

## Relationships

### Inherits From

- IOService

## See Also

### Power Management

IOACPIPlatformDevice

IOACPIPlatformExpert

IOPMPowerSource

IOPMPowerSourceList

IOPMrootDomain

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

