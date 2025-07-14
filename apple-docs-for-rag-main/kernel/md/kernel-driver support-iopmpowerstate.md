

- Kernel
- Driver Support
-  IOPMPowerState 

Structure

# IOPMPowerState

macOS 10.0+

``` source
typedef struct IOPMPowerState {
    ...
} IOPMPowerState;
```

## Topics

### Instance Properties

capabilityFlags

Describes the capability of the device in this state.

inputPowerRequirement

Describes the input power required in this state.

outputPowerCharacter

Describes the power provided in this state.

powerDomainBudget

Describes power in milliWatts a domain in this state can deliver to its children. Unused; drivers may specify 0. }

powerToAttain

Describes dditional power to attain this state from next lower state (in milliWatts). Unused; drivers may specify 0.

settleDownTime

Settle time required after entering next lower state from this state (microseconds). Unused; drivers may specify 0.

settleUpTime

Describes settle time required after entering this state from next lower state (microseconds). Unused; drivers may specify 0.

stateOrder

Valid in version kIOPMPowerStateVersion2 or greater of this structure. Defines ordering of power states independently of the power state ordinal.

staticPower

Describes average consumption in milliwatts. Unused; drivers may specify 0.

timeToAttain

Describes time required to enter this state from next lower state (in microseconds). Unused; drivers may specify 0.

timeToLower

Describes time required to enter next lower state from this one (microseconds). Unused; drivers may specify 0.

version

Defines version number of this struct. Just use the value "1" when defining an IOPMPowerState.

## See Also

### Power Management

IOACPIPlatformDevice

IOACPIPlatformExpert

IOPMPowerSource

IOPMPowerSourceList

IOPMrootDomain

IOPowerConnection

IOPwrController

IOACPIAddress

IOACPIAddressSpaceDescriptor

IOACPIAddressSpaceHandler

IOACPIAddressSpaceID

acknowledgeSleepWakeNotification

gIOACPIAddressKey

gIOACPIDeviceStatusKey

gIOACPIHardwareIDKey

gIOACPIPlane

gIOACPIUniqueIDKey

