

- IOUSBHost
- IOUSBHostCIPortStateMachine
-  respond(toCommand:status:) 

Instance Method

# respond(toCommand:status:)

Mac Catalyst 14.0+macOS 10.15+

``` source
func respond(
    toCommand command: UnsafePointer,
    status: IOUSBHostCIMessageStatus
) throws
```

## See Also

### Instance Methods

func inspectCommand(UnsafePointer&lt;IOUSBHostCIMessage>) throws

func updateLinkState(IOUSBHostCILinkState, speed: IOUSBHostCIDeviceSpeed, inhibitLinkStateChange: Bool) throws

