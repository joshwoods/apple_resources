

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- USB Device Descriptors
- IOUSBGetEndpointDescriptorOptions
-  kIOUSBGetEndpointDescriptorCurrentPolicy 

Enumeration Case

# kIOUSBGetEndpointDescriptorCurrentPolicy

The descriptor controlling the current endpoint policy.

macOS 10.15+

``` source
kIOUSBGetEndpointDescriptorCurrentPolicy
```

## Discussion

Specify this option when you want to include descriptor changes you made using the AdjustPipe method.

## See Also

### Getting the Options

kIOUSBGetEndpointDescriptorOriginal

The original descriptor that the system uses to create the pipe.

