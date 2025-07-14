

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- Additional Specifications
- USBReEnumerateOptions
-  kUSBAddExtraResetTimeBit 

Enumeration Case

# kUSBAddExtraResetTimeBit

Request extra time after reset.

macOS 10.3+

``` source
kUSBAddExtraResetTimeBit = 31
```

## Discussion

Setting this bit causes the hub driver to wait 100 milliseconds before addressing the device after the reset following the reenumeration.

