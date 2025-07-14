

- IOUSBHost
- IOUSBHostControllerInterface
-  enqueueInterrupts(\_:count:) 

Instance Method

# enqueueInterrupts(\_:count:)

Mac Catalyst 14.0+macOS 10.15+

``` source
func enqueueInterrupts(
    _ interrupts: UnsafePointer,
    count: Int
) throws
```

## See Also

### Instance Methods

func capabilities(forPort: Int) -> UnsafePointer&lt;IOUSBHostCIMessage>

func description(for: UnsafePointer&lt;IOUSBHostCIMessage>) -> String

func destroy()

func enqueueInterrupt(UnsafePointer&lt;IOUSBHostCIMessage>) throws

func enqueueInterrupt(UnsafePointer&lt;IOUSBHostCIMessage>, expedite: Bool) throws

func enqueueInterrupts(UnsafePointer&lt;IOUSBHostCIMessage>, count: Int, expedite: Bool) throws

func getPortStateMachine(forCommand: UnsafePointer&lt;IOUSBHostCIMessage>, error: NSErrorPointer) -> IOUSBHostCIPortStateMachine

func getPortStateMachine(forPort: Int, error: NSErrorPointer) -> IOUSBHostCIPortStateMachine

