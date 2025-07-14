

- PCIDriverKit
- IOPCIDevice
-  FindPCICapability 

Instance Method

# FindPCICapability

Search the configuration space for a PCI capability register.

DriverKitmacOS

``` source
kern_return_t FindPCICapability(uint32_t capabilityID, uint64_t searchOffset, uint64_t * foundCapabilityOffset);
```

## Parameters 

`capabilityID`  

A PCI capability ID. PCI Express devices may support extended capabilities in configuraiton space, starting at offset `0x100`. To search this space, pass an ID that is the negated value of the PCI-SIG assigned ID for the extended capability.

`searchOffset`  

The offset into configuration space at which to start the search.

`foundCapabilityOffset`  

A variable in which you want to store the resulting offset value.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Getting Device Information

GetBusDeviceFunction

Returns the device’s bus, device, and function numbers.

PCI Capabilities

Constants that you use to get the capabilities of the PCI device.

Slot Capabilities

Constants that you use to get the slot-related capabilities of the PCI device.

