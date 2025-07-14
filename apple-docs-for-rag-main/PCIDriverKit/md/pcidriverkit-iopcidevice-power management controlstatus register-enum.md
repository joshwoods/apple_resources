

- PCIDriverKit
- IOPCIDevice
-  Power Management Control/Status Register 

API Collection

# Power Management Control/Status Register

Constants you use when checking bits in the power management register.

## Topics

### Register Bits

kPCIPMCSPowerStateD0

The device is in the D0 state.

kPCIPMCSPowerStateD1

The device is in the D1 state.

kPCIPMCSPowerStateD2

The device is in the D2 state.

kPCIPMCSPowerStateD3

The device is in the D3 state.

kPCIPMCSPowerStateMask

A bit mask you use to determine the current power state of the device.

kPCIPMCSPMEEnable

The bit that specifies whether power management events are enabled.

kPCIPMCSPMEStatus

The bit that contains the current state of power management events.

kPCIPMCSDefaultEnableBits

The default power management settings.

kPCIPMCSPMEDisableInS3

A bit for a custom power management event.

kPCIPMCSPMEWakeReason

A bit that indicates the reason for waking the device.

## See Also

### Managing Power

HasPCIPowerManagement

Determines whether the device has the specified PCI bus power management capabilities.

EnablePCIPowerManagement

Configures the device’s PCI bus power management capabilities.

Power Management Capabilities

Constants you use to get and set the state of the device’s power management features.

