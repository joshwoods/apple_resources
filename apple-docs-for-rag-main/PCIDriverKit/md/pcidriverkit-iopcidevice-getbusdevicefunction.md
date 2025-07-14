

- PCIDriverKit
- IOPCIDevice
-  GetBusDeviceFunction 

Instance Method

# GetBusDeviceFunction

Returns the device’s bus, device, and function numbers.

DriverKitmacOS

``` source
kern_return_t GetBusDeviceFunction(uint8_t * returnBusNumber, uint8_t * returnDeviceNumber, uint8_t * returnFunctionNumber);
```

## Parameters 

`returnBusNumber`  

A variable in which you want to store the bus number.

`returnDeviceNumber`  

A variable in which you want to store the device number.

`returnFunctionNumber`  

A variable in which you want to store the function number.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Getting Device Information

FindPCICapability

Search the configuration space for a PCI capability register.

PCI Capabilities

Constants that you use to get the capabilities of the PCI device.

Slot Capabilities

Constants that you use to get the slot-related capabilities of the PCI device.

