

- Virtualization
- VZVirtualMachine
- VZVirtualMachine.State
-  VZVirtualMachine.State.paused 

Case

# VZVirtualMachine.State.paused

The framework has paused a started VM.

macOS 11.0+

``` source
case paused
```

## Discussion

The virtual machine can enter this state only from the VZVirtualMachine.State.pausing state.

## See Also

### States

case stopped

The VM isn’t running.

case running

The VM is running.

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

case error

The VM encountered an unrecoverable error.

case starting

The VM is configuring the hardware preparing to run.

case pausing

The VM is pausing.

case stopping

The VM is stopping.

