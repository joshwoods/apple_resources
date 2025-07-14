

- Virtualization
- VZVirtualMachine
- VZVirtualMachine.State
-  VZVirtualMachine.State.error 

Case

# VZVirtualMachine.State.error

The VM encountered an unrecoverable error.

macOS 11.0+

``` source
case error
```

## Discussion

The VM encountered an unrecoverable error and the framework can no longer use the VM; you need to destroy the VZVirtualMachine object.

## See Also

### States

case stopped

The VM isn’t running.

case running

The VM is running.

case paused

The framework has paused a started VM.

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

case starting

The VM is configuring the hardware preparing to run.

case pausing

The VM is pausing.

case stopping

The VM is stopping.

