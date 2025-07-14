

- PCIDriverKit
- IOPCIDevice
-  PCI Capabilities 

API Collection

# PCI Capabilities

Constants that you use to get the capabilities of the PCI device.

## Topics

### Capability Bits

kIOPCICapabilityIDOffset

The offset to the location of the device’s capability ID.

kIOPCINextCapabilityOffset

The offset to the next PCI capability structure.

kIOPCICapabilityIDPowerManagement

The identifier for the power management interface.

kIOPCICapabilityIDAGP

The identifier for the AGP capability.

kIOPCICapabilityIDVitalProductData

The identifier for the vital product data capability.

kIOPCICapabilityIDSlotID

The identifier for the slot identification capability.

kIOPCICapabilityIDMSI

The identifier for the MSI capability.

kIOPCICapabilityIDCPCIHotswap

The identifier for the CompactPCI hot swap capability.

kIOPCICapabilityIDPCIX

The identifier for the PCI-X capability.

kIOPCICapabilityIDLDT

The identifier for the HyperTransport capability.

kIOPCICapabilityIDVendorSpecific

The identifier for any vendor-specific capabilities.

kIOPCICapabilityIDDebugPort

The identifier for the debug port capability.

kIOPCICapabilityIDCPCIResourceControl

The identifier for the CompactPCI central resource control capability.

kIOPCICapabilityIDHotplug

The identifier for the PCI hot plug capability.

kIOPCICapabilityIDAGP8

The identifier for the AGP 8x capability.

kIOPCICapabilityIDSecure

The identifer for the secure device capability.

kIOPCICapabilityIDPCIExpress

The identifier for the PCI Express capability.

kIOPCICapabilityIDMSIX

The identifer for the MSI-X capability.

kIOPCICapabilityIDFPB

The identifier for the flattening portal bridge capability.

kIOPCIExpressCapabilityIDErrorReporting

The identifier for the advanced error reporting extended capability.

kIOPCIExpressCapabilityIDVirtualChannel

The identifier for the virtual channel extended capability.

kIOPCIExpressCapabilityIDDeviceSerialNumber

The identifier for the device serial number extended capability.

kIOPCIExpressCapabilityIDPowerBudget

The identifier for the power budgeting extended capability.

kIOPCIExpressCapabilityIDAccessControlServices

The identifier for the access control services extended capability.

kIOPCIExpressCapabilityIDLatencyTolerenceReporting

The identifier for the latency tolerance reporting extended capability.

kIOPCIExpressCapabilityIDL1PMSubstates

The identifier for the L1 power management substates extended capability.

### Constants

kIOPCIExpressCapabilityIDAlternativeRoutingID

kIOPCIExpressCapabilityIDPrecisionTimeManagement

## See Also

### Getting Device Information

FindPCICapability

Search the configuration space for a PCI capability register.

GetBusDeviceFunction

Returns the device’s bus, device, and function numbers.

Slot Capabilities

Constants that you use to get the slot-related capabilities of the PCI device.

