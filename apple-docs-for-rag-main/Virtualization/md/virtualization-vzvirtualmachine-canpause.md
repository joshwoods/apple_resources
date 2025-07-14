

- Virtualization
- VZVirtualMachine
-  canPause 

Instance Property

# canPause

A Boolean value that indicates whether you can pause the VM.

macOS 11.0+

``` source
var canPause: Bool { get }
```

## Discussion

The value of this property is true when the VM is in a state that allows you to pause it. Call the pause(completionHandler:) method (Swift) or pause() method (Objective-C) to pause the VM.

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

var canResume: Bool

A Boolean value that indicates whether you can resume the VM.

var canStop: Bool

A Boolean value that indicates whether you can stop the VM.

var canRequestStop: Bool

A Boolean value that indicates whether you can ask the guest operating system to stop running.

