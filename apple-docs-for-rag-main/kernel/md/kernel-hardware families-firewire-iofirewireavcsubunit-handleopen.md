

- Kernel
- Hardware Families
- FireWire
- IOFireWireAVCSubUnit
-  handleOpen 

# handleOpen

Overrideable method to control the open / close behaviour of an IOService.

``` source
virtual bool handleOpen(
 IOService *forClient, 
 IOOptionBits options, 
 void *arg ); 
```

## Parameters 

`forClient`  

Designates the client of the provider requesting the open.

`options`  

Options for the open, may be interpreted by the implementor of handleOpen.

## Return Value

Return true if the open was successful, false otherwise.

## Overview

See IOService for discussion.

## See Also

### Miscellaneous

AVCCommand

Sends an AVC command to the device and stores the response.

AVCCommandInGeneration

Sends an AVC command to the device and stores the response. The command must complete in the specified FireWire bus generation otherwise kIOFireWireBusReset is returned.

handleClose

Overrideable method to control the open / close behaviour of an IOService.

matchPropertyTable

Matching language support Match on the following properties of the sub unit: Vendor_ID GUID SubUnit_Type

updateAVCCommandTimeout

By default, AVCCommands timeout 10 seconds after receiving an Interim response. This function resets the timeout of the current command to 10 seconds from the current time. Call this repeatedly for AVC commands that take a very long time to execute to prevent premature timeout.

