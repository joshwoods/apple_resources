

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- Additional Specifications
- USBPowerRequestTypes
-  kUSBPowerRequestWakeRelease 

Enumeration Case

# kUSBPowerRequestWakeRelease

The system requests a release of power upon waking.

macOS 10.7+

``` source
kUSBPowerRequestWakeRelease = 2
```

## Discussion

When you use this enumeration with ReturnExtraPower, it sends a message to all devices to return any extra wake power, if possible.

