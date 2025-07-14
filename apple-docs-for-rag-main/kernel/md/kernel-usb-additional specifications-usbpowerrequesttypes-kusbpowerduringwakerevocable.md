

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- Additional Specifications
- USBPowerRequestTypes
-  kUSBPowerDuringWakeRevocable 

Enumeration Case

# kUSBPowerDuringWakeRevocable

The system requests power reallocation as revocable.

macOS 10.8+

``` source
kUSBPowerDuringWakeRevocable = 6
```

## Discussion

The system uses this extra power while it’s awake, but the kUSBPowerRequestWakeRelease message can take that power away and reallocate it to another device.

