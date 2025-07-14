

- IOUSBHost
- IOUSBHostCIEndpointStateMachine
-  processDoorbell(\_:) 

Instance Method

# processDoorbell(\_:)

Mac Catalyst 14.0+macOS 10.15+

``` source
func processDoorbell(_ doorbell: IOUSBHostCIDoorbell) throws
```

## See Also

### Instance Methods

func enqueueTransferCompletion(for: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus, transferLength: Int) throws

func inspectCommand(UnsafePointer&lt;IOUSBHostCIMessage>) throws

func respond(toCommand: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus) throws

