

- Virtualization
- VZDiskSynchronizationMode
-  VZDiskSynchronizationMode.full 

Case

# VZDiskSynchronizationMode.full

Perform all synchronization operations as requested by the guest OS.

macOS 14.0+

``` source
case full
```

## Discussion

Using this mode, `flush` and `barrier` commands from the guest result in the system sending their counterpart synchronization commands to the underlying disk implementation.

## See Also

### Synchronization modes

case none

Don’t synchronize the data with the permanent storage.

