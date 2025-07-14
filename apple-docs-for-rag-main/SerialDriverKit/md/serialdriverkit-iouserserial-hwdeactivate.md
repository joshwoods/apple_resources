

- SerialDriverKit
- IOUserSerial
-  HwDeactivate 

Instance Method

# HwDeactivate

Closes the communication channel to the device.

DriverKit 19.0+

``` source
kern_return_t HwDeactivate();
```

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Override this method as needed and use it to close the connection to your device’s hardware. Always call the `super` version of the method at the end of your implementation.

## See Also

### Activating and Deactivating the Service

HwActivate

Opens the communication channel to the device.

