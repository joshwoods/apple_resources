

- IOUSBHost
- IOUSBHostCIControllerStateMachine
-  respond(toCommand:status:frame:timestamp:) 

Instance Method

# respond(toCommand:status:frame:timestamp:)

Mac Catalyst 14.0+macOS 10.15+

``` source
func respond(
    toCommand command: UnsafePointer,
    status: IOUSBHostCIMessageStatus,
    frame: UInt64,
    timestamp: UInt64
) throws
```

## See Also

### Instance Methods

func enqueueUpdatedFrame(UInt64, timestamp: UInt64) throws

func inspectCommand(UnsafePointer&lt;IOUSBHostCIMessage>) throws

func respond(toCommand: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus) throws

