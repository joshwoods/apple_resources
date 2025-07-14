

- Kernel
- IOKit Fundamentals
- Memory
- IODeviceMemory
-  InitElement 

# InitElement

``` source
struct InitElement {
   IOPhysicalAddress start;
   IOPhysicalLength length;
   IOOptionBits tag;
};
```

## Topics

### Fields

start

First physical address in the range.

length

Length of the range.

tag

32-bit value not interpreted by IODeviceMemory or IOMemoryDescriptor, for use by the bus family.

