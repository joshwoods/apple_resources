

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- Additional Specifications
- USBPowerRequestTypes
-  kUSBPowerRequestWakeReallocate 

Enumeration Case

# kUSBPowerRequestWakeReallocate

The system requests power reallocation upon waking.

macOS 10.7+

``` source
kUSBPowerRequestWakeReallocate = 4
```

## Discussion

When you use this enumeration with ReturnExtraPower, it sends a message to all devices to return more wake power because some devices have released it.

