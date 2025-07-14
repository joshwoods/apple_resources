

- Kernel
- Kernel Enumerations
- Anonymous
-  kIOPMInitialDeviceState 

Enumeration Case

# kIOPMInitialDeviceState

macOS 10.12+

``` source
kIOPMInitialDeviceState = 0x00000100
```

## Discussion

Indicates the initial power state for the device. If `initialPowerStateForDomainState()` returns a power state with this flag set in the capability field, then the initial power change is performed without calling the driver's `setPowerState()`.

