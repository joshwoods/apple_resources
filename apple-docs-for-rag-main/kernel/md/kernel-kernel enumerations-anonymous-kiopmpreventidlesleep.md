

- Kernel
- Kernel Enumerations
- Anonymous
-  kIOPMPreventIdleSleep 

Enumeration Case

# kIOPMPreventIdleSleep

macOS 10.12+

``` source
kIOPMPreventIdleSleep = 0x00000040
```

## Discussion

In the capability field of a power state, disallows idle system sleep while the device is in that state.

For example, displays and disks set this capability for their ON power state; since the system may not idle sleep while the display (and thus keyboard or mouse) or the disk is active.

Useful only as a Capability.

