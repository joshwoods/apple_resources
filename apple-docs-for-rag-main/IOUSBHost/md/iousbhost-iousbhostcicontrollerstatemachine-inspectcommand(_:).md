

- IOUSBHost
- IOUSBHostCIControllerStateMachine
-  inspectCommand(\_:) 

Instance Method

# inspectCommand(\_:)

Mac Catalyst 14.0+macOS 10.15+

``` source
func inspectCommand(_ command: UnsafePointer) throws
```

## See Also

### Instance Methods

func enqueueUpdatedFrame(UInt64, timestamp: UInt64) throws

func respond(toCommand: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus) throws

func respond(toCommand: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus, frame: UInt64, timestamp: UInt64) throws

