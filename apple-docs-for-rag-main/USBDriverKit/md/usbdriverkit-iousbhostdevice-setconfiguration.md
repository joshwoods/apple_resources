

- USBDriverKit
- IOUSBHostDevice
-  SetConfiguration 

Instance Method

# SetConfiguration

Selects a new configuration for the device.

DriverKit 19.0+

``` source
kern_return_t SetConfiguration(uint8_t bConfigurationValue, bool matchInterfaces);
```

## Parameters 

`bConfigurationValue`  

The configuration to select. You can get this value from the bConfigurationValue field of the IOUSBConfigurationDescriptor structure.

`matchInterfaces`  

A Boolean value indicating whether you want the system to perform matching on the interfaces of the new configuration. Specify false to skip the matching process.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

This method terminates all previously configured child interfaces and sets the new configuration for the device. This method sends a `SET_CONFIGURATION` control request (USB 2.0, section 9.4.7) to the device. When making the `GET_DESCRIPTOR` control request, this method acquires the service’s workloop lock and may call commandSleep.

