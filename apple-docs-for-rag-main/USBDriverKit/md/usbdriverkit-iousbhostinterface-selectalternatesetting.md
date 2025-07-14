

- USBDriverKit
- IOUSBHostInterface
-  SelectAlternateSetting 

Instance Method

# SelectAlternateSetting

Selects an alternative setting for this interface.

DriverKit 19.0+

``` source
kern_return_t SelectAlternateSetting(uint8_t bAlternateSetting);
```

## Parameters 

`bAlternateSetting`  

The alternative interface number to activate.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Use this method to select an alternative setting for the interface. The system aborts all pending I/O on the interface’s pipes, and closes any open pipes. The system selects the new alternative setting using the `SET_INTERFACE` control request (USB 2.0, section 9.4.10).

## See Also

### Configuring the Interface

GetFrameNumber

Gets the current frame number of the USB controller.

GetPortStatus

Gets the current port status.

GetIdlePolicy

Gets the current idle suspend timeout for the interface.

SetIdlePolicy

Sets the desired idle suspend timeout for the interface.

tIOUSBHostPortStatus

Constants indicating the state of a port.

