

- IOUSBHost
- IOUSBHostCIControllerStateMachine
-  enqueueUpdatedFrame(\_:timestamp:) 

Instance Method

# enqueueUpdatedFrame(\_:timestamp:)

Mac Catalyst 14.0+macOS 10.15+

``` source
func enqueueUpdatedFrame(
    _ frame: UInt64,
    timestamp: UInt64
) throws
```

## See Also

### Instance Methods

func inspectCommand(UnsafePointer&lt;IOUSBHostCIMessage>) throws

func respond(toCommand: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus) throws

func respond(toCommand: UnsafePointer&lt;IOUSBHostCIMessage>, status: IOUSBHostCIMessageStatus, frame: UInt64, timestamp: UInt64) throws

