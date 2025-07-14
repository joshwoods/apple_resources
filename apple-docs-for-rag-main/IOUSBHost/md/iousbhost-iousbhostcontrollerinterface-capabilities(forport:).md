

- IOUSBHost
- IOUSBHostControllerInterface
-  capabilities(forPort:) 

Instance Method

# capabilities(forPort:)

Mac Catalyst 14.0+macOS 10.15+

``` source
func capabilities(forPort port: Int) -> UnsafePointer
```

## See Also

### Instance Methods

func description(for: UnsafePointer&lt;IOUSBHostCIMessage>) -> String

func destroy()

func enqueueInterrupt(UnsafePointer&lt;IOUSBHostCIMessage>) throws

func enqueueInterrupt(UnsafePointer&lt;IOUSBHostCIMessage>, expedite: Bool) throws

func enqueueInterrupts(UnsafePointer&lt;IOUSBHostCIMessage>, count: Int) throws

func enqueueInterrupts(UnsafePointer&lt;IOUSBHostCIMessage>, count: Int, expedite: Bool) throws

func getPortStateMachine(forCommand: UnsafePointer&lt;IOUSBHostCIMessage>, error: NSErrorPointer) -> IOUSBHostCIPortStateMachine

func getPortStateMachine(forPort: Int, error: NSErrorPointer) -> IOUSBHostCIPortStateMachine

