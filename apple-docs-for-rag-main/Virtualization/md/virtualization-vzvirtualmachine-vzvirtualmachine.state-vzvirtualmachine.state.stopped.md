

- Virtualization
- VZVirtualMachine
- VZVirtualMachine.State
-  VZVirtualMachine.State.stopped 

Case

# VZVirtualMachine.State.stopped

The VM isn’t running.

macOS 11.0+

``` source
case stopped
```

## Mentioned in 

Installing macOS on a Virtual Machine

## Discussion

This state is the initial state of the virtual machine.

## See Also

### States

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

