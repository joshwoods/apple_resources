

- IOUSBHost
- IOUSBHostCIPortStateMachine
-  updateLinkState(\_:speed:inhibitLinkStateChange:) 

Instance Method

# updateLinkState(\_:speed:inhibitLinkStateChange:)

Mac Catalyst 14.0+macOS 10.15+

``` source
func updateLinkState(
    _ linkState: IOUSBHostCILinkState,
    speed: IOUSBHostCIDeviceSpeed,
    inhibitLinkStateChange: Bool
) throws
```

## See Also

### Instance Methods

func inspectCommand(UnsafePointer&lt;IOUSBHostCIMessage>) throws

func respond(toCommand: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus) throws

