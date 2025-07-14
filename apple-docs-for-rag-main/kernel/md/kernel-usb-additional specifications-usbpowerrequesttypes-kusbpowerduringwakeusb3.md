

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- Additional Specifications
- USBPowerRequestTypes
-  kUSBPowerDuringWakeUSB3 

Enumeration Case

# kUSBPowerDuringWakeUSB3

The system requests extra power allocation.

macOS 10.8+

``` source
kUSBPowerDuringWakeUSB3 = 7
```

## Discussion

The USB stack uses this enumeration to allocate the 400 milliamps extra for USB 3.0 above the 500 milliamps that USB 2.0 allocates.

