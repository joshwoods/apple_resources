

- Virtualization
- VZVirtualMachine
- VZVirtualMachine.State
-  VZVirtualMachine.State.stopping 

Case

# VZVirtualMachine.State.stopping

The VM is stopping.

macOS 12.0+

``` source
case stopping
```

## Discussion

This is the intermediate state between VZVirtualMachine.State.running and VZVirtualMachine.State.stopped.

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

