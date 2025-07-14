

- IOUSBHost
- IOUSBHostCIDeviceStateMachine
-  respond(toCommand:status:deviceAddress:) 

Instance Method

# respond(toCommand:status:deviceAddress:)

Mac Catalyst 14.0+macOS 10.15+

``` source
func respond(
    toCommand command: UnsafePointer,
    status: IOUSBHostCIMessageStatus,
    deviceAddress: Int
) throws
```

## See Also

### Instance Methods

func inspectCommand(UnsafePointer&lt;IOUSBHostCIMessage>) throws

func respond(toCommand: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus) throws

