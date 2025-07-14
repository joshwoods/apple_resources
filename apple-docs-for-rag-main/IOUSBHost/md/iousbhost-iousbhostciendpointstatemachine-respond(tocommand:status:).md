

- IOUSBHost
- IOUSBHostCIEndpointStateMachine
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

func enqueueTransferCompletion(for: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus, transferLength: Int) throws

func inspectCommand(UnsafePointer&lt;IOUSBHostCIMessage>) throws

func processDoorbell(IOUSBHostCIDoorbell) throws

