

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- Additional Specifications
- USBPowerRequestTypes
-  kUSBPowerRequestSleepRelease 

Enumeration Case

# kUSBPowerRequestSleepRelease

The system requests a release of power upon sleeping.

macOS 10.7+

``` source
kUSBPowerRequestSleepRelease = 3
```

## Discussion

When you use this enumeration with ReturnExtraPower, it sends a message to all devices to return any sleep power, if possible.

