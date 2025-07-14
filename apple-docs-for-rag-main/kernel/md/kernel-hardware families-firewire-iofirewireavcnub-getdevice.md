

- Kernel
- Hardware Families
- FireWire
- IOFireWireAVCNub
-  getDevice 

# getDevice

Returns the FireWire device nub that is this object's provider .

``` source
IOFireWireNub* getDevice() const ;
```

## See Also

### Miscellaneous

AVCCommand

Sends an AVC command to the device and stores the response.

AVCCommandInGeneration

Sends an AVC command to the device and stores the response. The command must complete in the specified FireWire bus generation otherwise kIOFireWireBusReset is returned.

updateAVCCommandTimeout

By default, AVCCommands timeout 10 seconds after receiving an Interim response. This function resets the timeout of the current command to 10 seconds from the current time. Call this repeatedly for AVC commands that take a very long time to execute to prevent premature timeout.

