

- Virtualization
- VZVirtualMachine
- VZVirtualMachine.State
-  VZVirtualMachine.State.resuming 

Case

# VZVirtualMachine.State.resuming

The VM is resuming from a paused state.

macOS 11.0+

``` source
case resuming
```

## Discussion

This state is an intermediate state between the VZVirtualMachine.State.paused and VZVirtualMachine.State.running states.

## See Also

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

