

- Virtualization
- VZVirtualMachine
-  canRequestStop 

Instance Property

# canRequestStop

A Boolean value that indicates whether you can ask the guest operating system to stop running.

macOS 11.0+

``` source
var canRequestStop: Bool { get }
```

## Discussion

The value of this property is true when the VM is in a state that allows it to stop running. Call the requestStop() method to ask the guest operating system to stop running.

## See Also

### Getting the state of the VM

var state: VZVirtualMachine.State

The current execution state of the VM.

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

