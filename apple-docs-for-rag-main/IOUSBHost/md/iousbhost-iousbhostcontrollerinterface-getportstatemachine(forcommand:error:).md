

- IOUSBHost
- IOUSBHostControllerInterface
-  getPortStateMachine(forCommand:error:) 

Instance Method

# getPortStateMachine(forCommand:error:)

Mac Catalyst 14.0+macOS 10.15+

``` source
func getPortStateMachine(
    forCommand command: UnsafePointer,
    error: NSErrorPointer
) -> IOUSBHostCIPortStateMachine
```

## See Also

### Instance Methods

func capabilities(forPort: Int) -> UnsafePointer&lt;IOUSBHostCIMessage>

func description(for: UnsafePointer&lt;IOUSBHostCIMessage>) -> String

func destroy()

func enqueueInterrupt(UnsafePointer&lt;IOUSBHostCIMessage>) throws

func enqueueInterrupt(UnsafePointer&lt;IOUSBHostCIMessage>, expedite: Bool) throws

func enqueueInterrupts(UnsafePointer&lt;IOUSBHostCIMessage>, count: Int) throws

func enqueueInterrupts(UnsafePointer&lt;IOUSBHostCIMessage>, count: Int, expedite: Bool) throws

func getPortStateMachine(forPort: Int, error: NSErrorPointer) -> IOUSBHostCIPortStateMachine

