

- USBDriverKit
- IOUSBHostInterface
-  SetIdlePolicy 

Instance Method

# SetIdlePolicy

Sets the desired idle suspend timeout for the interface.

DriverKit 19.0+

``` source
kern_return_t SetIdlePolicy(uint32_t deviceIdleTimeout);
```

## Parameters 

`deviceIdleTimeout`  

The amount of time, in milliseconds, to wait after all pipes are idle before suspending the device. It is recommended that you choose an idle timeout value of 50 milliseconds or larger.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

An idle device defers electrical suspension for the specified duration. By default, IOUSBHostInterface doesn’t enable an idle policy, letting the device remain in the active state as long as the host machine is awake. Call this method to enable an idle policy for your device.

When you enable an idle policy and no I/O requests are pending, the system waits for the specified amount of time before electrically suspending the device. For a device with multiple interfaces, the system uses the largest timeout value from among all the open interfaces. A new I/O request during the wait period, or after suspension occurs, cancels the suspension and resumes I/O operations.

If the parent IOUSBHostDevice object does not allow low-power mode for the device, the system disables idle suspension altogether.

## See Also

### Configuring the Interface

GetFrameNumber

Gets the current frame number of the USB controller.

GetPortStatus

Gets the current port status.

SelectAlternateSetting

Selects an alternative setting for this interface.

GetIdlePolicy

Gets the current idle suspend timeout for the interface.

tIOUSBHostPortStatus

Constants indicating the state of a port.

