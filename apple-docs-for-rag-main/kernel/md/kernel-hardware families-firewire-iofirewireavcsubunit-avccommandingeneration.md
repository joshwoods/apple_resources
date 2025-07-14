

- Kernel
- Hardware Families
- FireWire
- IOFireWireAVCSubUnit
-  AVCCommandInGeneration 

# AVCCommandInGeneration

Sends an AVC command to the device and stores the response. The command must complete in the specified FireWire bus generation otherwise kIOFireWireBusReset is returned.

``` source
virtual IOReturn AVCCommandInGeneration(
 UInt32generation, 
 const UInt8 *command,
 UInt32cmdLen,
 UInt8 *response,
 UInt32 *responseLen); 
```

## Parameters 

`generation`  

The bus generation that the command must execute in.

`command`  

Pointer to command to send.

`cmdLen`  

Length of the command.

`response`  

Pointer to place to store the response.

`responseLen`  

Pointer to response length - initialize to the size of the buffer pointed to by response, updated to the number of bytes returned by the device.

## See Also

### Miscellaneous

AVCCommand

Sends an AVC command to the device and stores the response.

handleClose

Overrideable method to control the open / close behaviour of an IOService.

handleOpen

Overrideable method to control the open / close behaviour of an IOService.

matchPropertyTable

Matching language support Match on the following properties of the sub unit: Vendor_ID GUID SubUnit_Type

updateAVCCommandTimeout

By default, AVCCommands timeout 10 seconds after receiving an Interim response. This function resets the timeout of the current command to 10 seconds from the current time. Call this repeatedly for AVC commands that take a very long time to execute to prevent premature timeout.

