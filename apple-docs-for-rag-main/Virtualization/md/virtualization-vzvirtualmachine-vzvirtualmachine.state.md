

- Virtualization
- VZVirtualMachine
-  VZVirtualMachine.State 

Enumeration

# VZVirtualMachine.State

The execution states of the VM.

macOS 11.0+

``` source
enum State
```

## Topics

### States

case stopped

The VM isn’t running.

case running

The VM is running.

case paused

The framework has paused a started VM.

case error

The VM encountered an unrecoverable error.

case starting

The VM is configuring the hardware preparing to run.

case pausing

The VM is pausing.

case stopping

The VM is stopping.

case resuming

The VM is resuming from a paused state.

case restoring

The VM is restoring from a saved state.

case saving

The VM is saving its state.

case stopped

The VM isn’t running.

case running

The VM is running.

case paused

The framework has paused a started VM.

case error

The VM encountered an unrecoverable error.

case starting

The VM is configuring the hardware preparing to run.

case pausing

The VM is pausing.

case stopping

The VM is stopping.

case resuming

The VM is resuming from a paused state.

case restoring

The VM is restoring from a saved state.

case saving

The VM is saving its state.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the state of the VM

var state: VZVirtualMachine.State

The current execution state of the VM.

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

