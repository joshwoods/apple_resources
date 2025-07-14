

- Kernel
- Driver Support
-  IOACPIAddressSpaceHandler 

Type Alias

# IOACPIAddressSpaceHandler

macOS 10.3+

``` source
typedef IOReturn (*IOACPIAddressSpaceHandler)(UInt32 operation, IOACPIAddress address, UInt64 *value, UInt32 bitWidth, UInt32 bitOffset, void *context);
```

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

IOACPIAddressSpaceID

IOPMPowerState

acknowledgeSleepWakeNotification

gIOACPIAddressKey

gIOACPIDeviceStatusKey

gIOACPIHardwareIDKey

gIOACPIPlane

gIOACPIUniqueIDKey

