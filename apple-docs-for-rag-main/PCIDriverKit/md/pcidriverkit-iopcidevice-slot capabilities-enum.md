

- PCIDriverKit
- IOPCIDevice
-  Slot Capabilities 

API Collection

# Slot Capabilities

Constants that you use to get the slot-related capabilities of the PCI device.

## Topics

### Capabilities

kIOPCISlotCapabilitiesBitAttentionButtonPresent

The bit that indicates whether an attention button for this slot is electrically controlled by the chassis.

kIOPCISlotCapabilitiesBitPowerControllerPresent

The bit that indicates whether the slot implements a software programmable power controller.

kIOPCISlotCapabilitiesBitMRLSensorPresent

The bit that indicates whether the chassis for this slot implements an MRL sensor.

kIOPCISlotCapabilitiesBitAttentionIndicatorPresent

The bit that indicates whether the chassis electrically controls the attention indicator.

kIOPCISlotCapabilitiesBitPowerIndicatorPresent

The bit that indicates whether chassis electrically controls the power indicator.

kIOPCISlotCapabilitiesBitHotPlugSurprise

The bit that indicates whether the adaptor might be removed without prior notification.

kIOPCISlotCapabilitiesBitHotPlugCapable

The bit that indicates whether the slot supports hot-plug operations.

kIOPCISlotCapabilitiesBitElectromechanicalInterlockPresent

The bit that indicates whether the chassis implements an electromechanical interlock for this slot.

kIOPCISlotCapabilitiesBitNoCommandCompletedSupport

The bit that indicates whether the slot generates a software notification when the Hot-Plug controller finishes a command.

## See Also

### Getting Device Information

FindPCICapability

Search the configuration space for a PCI capability register.

GetBusDeviceFunction

Returns the device’s bus, device, and function numbers.

PCI Capabilities

Constants that you use to get the capabilities of the PCI device.

