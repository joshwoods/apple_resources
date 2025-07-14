

- IOUSBHost
- IOUSBHostCIEndpointStateMachine
-  enqueueTransferCompletion(for:status:transferLength:) 

Instance Method

# enqueueTransferCompletion(for:status:transferLength:)

Mac Catalyst 14.0+macOS 10.15+

``` source
func enqueueTransferCompletion(
    for message: UnsafePointer,
    status: IOUSBHostCIMessageStatus,
    transferLength: Int
) throws
```

## See Also

### Instance Methods

func inspectCommand(UnsafePointer&lt;IOUSBHostCIMessage>) throws

func processDoorbell(IOUSBHostCIDoorbell) throws

func respond(toCommand: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus) throws

