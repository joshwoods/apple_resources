

- IOUSBHost
- IOUSBHostCIEndpointStateMachine
-  inspectCommand(\_:) 

Instance Method

# inspectCommand(\_:)

Mac Catalyst 14.0+macOS 10.15+

``` source
func inspectCommand(_ command: UnsafePointer) throws
```

## See Also

### Instance Methods

func enqueueTransferCompletion(for: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus, transferLength: Int) throws

func processDoorbell(IOUSBHostCIDoorbell) throws

func respond(toCommand: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus) throws

