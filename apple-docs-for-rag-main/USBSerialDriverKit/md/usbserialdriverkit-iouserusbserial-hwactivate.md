

- USBSerialDriverKit
- IOUserUSBSerial
-  HwActivate 

Instance Method

# HwActivate

Opens the communication channel to the device.

DriverKit 19.0+

``` source
kern_return_t HwActivate();
```

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Override this method and use it to prepare your device’s hardware for serial communication. Always call the `super` version of the method at the beginning of your implementation.

## See Also

### Activating and Deactivating the Service

HwDeactivate

Closes the communication channel to the device.

