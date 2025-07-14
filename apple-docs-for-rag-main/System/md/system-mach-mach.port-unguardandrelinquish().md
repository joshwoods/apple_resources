

- System
- Mach
- Mach.Port
-  unguardAndRelinquish() 

Instance Method

# unguardAndRelinquish()

Remove guard and transfer ownership of the underlying port right to the caller.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.0+watchOS 10.4+

``` source
consuming func unguardAndRelinquish() -> mach_port_name_t
```

Available when `RightType` is `Mach.ReceiveRight`.

## Discussion

Returns the Mach port name representing the right.

This operation liberates the right from management by the Mach.Port, and the underlying right will no longer be automatically deallocated.

After this function completes, the Mach.Port is destroyed and no longer usable.

This function makes a syscall to remove the guard from Mach.ReceiveRights. Use relinquish() to avoid the syscall and extract the context value along with the port name.

