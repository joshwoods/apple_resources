

- Virtualization
- VZVirtualMachine
-  state 

Instance Property

# state

The current execution state of the VM.

macOS 11.0+

``` source
var state: VZVirtualMachine.State { get }
```

## See Also

### Getting the state of the VM

enum State

The execution states of the VM.

var graphicsDevices: [VZGraphicsDevice]

The list of configured graphics devices on the virtual machine.

var canStart: Bool

A Boolean value that indicates whether you can start the VM.

var canPause: Bool

A Boolean value that indicates whether you can pause the VM.

var canResume: Bool

A Boolean value that indicates whether you can resume the VM.

var canStop: Bool

A Boolean value that indicates whether you can stop the VM.

var canRequestStop: Bool

A Boolean value that indicates whether you can ask the guest operating system to stop running.

