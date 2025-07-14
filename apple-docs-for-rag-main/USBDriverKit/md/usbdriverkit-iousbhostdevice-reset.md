

- USBDriverKit
- IOUSBHostDevice
-  Reset 

Instance Method

# Reset

Terminates the device and attempts to reenumerate it.

DriverKit 19.0+

``` source
kern_return_t Reset();
```

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

This method resets and releases the current IOUSBHostDevice object and all of its children. If the reset and release of the device object are successful, this method creates a new IOUSBHostDevice object and registers it.

Don’t call this function from the port workloop thread.

## See Also

### Managing the Device Session

Open

Opens a session to a host device.

Close

Closes the session to the host device.

