

- Kernel
- Driver Support
-  IOACPIPlatformDevice 

Class

# IOACPIPlatformDevice

macOS 10.3+

``` source
class IOACPIPlatformDevice : IOPlatformDevice
```

## Topics

### Instance Methods

- acquireGlobalLock

- attachToParent

- compareName

- detachFromParent

- evaluateInteger

- evaluateInteger

- evaluateInteger

- evaluateInteger

- evaluateObject

- evaluateObject

- free

- getACPITableData

- getDeviceHandle

- getDeviceStatus

- getDeviceType

- getMetaClass

- getPathComponent

- getResources

- hasACPIPowerStateSupport

- hasSystemWakeCapability

- init

- initACPIPowerManagement

- installInterruptForFixedEvent

- installInterruptForGPE

- ioRead16

- ioRead32

- ioRead8

- ioWrite16

- ioWrite32

- ioWrite8

- readAddressSpace

- registerAddressSpaceHandler

- releaseGlobalLock

- setACPIPowerManagementEnable

- setDeviceType

- setPowerState

- setSystemWakeCapabilityEnable

- stopACPIPowerManagement

- unregisterAddressSpaceHandler

- validateObject

- validateObject

- writeAddressSpace

## Relationships

### Inherits From

- IOPlatformDevice

## See Also

### Power Management

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

IOPMPowerState

acknowledgeSleepWakeNotification

gIOACPIAddressKey

gIOACPIDeviceStatusKey

gIOACPIHardwareIDKey

gIOACPIPlane

gIOACPIUniqueIDKey

