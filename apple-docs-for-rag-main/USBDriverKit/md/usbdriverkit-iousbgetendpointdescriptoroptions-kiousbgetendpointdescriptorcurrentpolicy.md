

- USBDriverKit
- IOUSBGetEndpointDescriptorOptions
-  kIOUSBGetEndpointDescriptorCurrentPolicy 

Enumeration Case

# kIOUSBGetEndpointDescriptorCurrentPolicy

The descriptor controlling the current endpoint policy.

DriverKit 19.0+

``` source
kIOUSBGetEndpointDescriptorCurrentPolicy
```

## Discussion

Specify this option when you want the include descriptor changes you made using the AdjustPipe method.

## See Also

### Getting the Descriptor Options

kIOUSBGetEndpointDescriptorOriginal

The original descriptor used to create the pipe.

