

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- Additional Specifications
- USBPowerRequestTypes
-  kUSBPowerRequestSleepReallocate 

Enumeration Case

# kUSBPowerRequestSleepReallocate

The system requests power reallocation upon sleeping.

macOS 10.7+

``` source
kUSBPowerRequestSleepReallocate = 5
```

## Discussion

When you use this enumeration with ReturnExtraPower, it sends a message to all devices to return more sleep power because some devices have released it.

