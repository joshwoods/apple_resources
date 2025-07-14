

- IOUSBHost
- IOUSBHostDevice
-  reset() 

Instance Method

# reset()

Terminates the device and attempts to re-enumerate it.

Mac Catalyst 14.0+macOS 10.15+

``` source
func reset() throws
```

## Discussion

This function resets and attempts to re-enumerate the USB device, and terminates the IOUSBHostDevice and all of its child IOService objects. If the reset is successful, it also creates and registers a new IOService object after terminating the previous object. After the call returns successfully, the framework IOUSBHostDevice no longer has a valid connection with the IOService object.

Important

To use the re-enumerated device, you must create a new framework client using initWithIOService:options:queue:error:interestHandler:.

