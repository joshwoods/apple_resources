

- USBDriverKit
- IOUSBBOSDescriptor
-  bDescriptorType 

Instance Property

# bDescriptorType

The type of the descriptor.

DriverKit 19.0+

``` source
uint8_t bDescriptorType;
```

## Discussion

The value in this field is always kIOUSBDescriptorTypeBOS.

## See Also

### Accessing the Descriptor Properties

bLength

The size of the descriptor in bytes.

wTotalLength

The length, in bytes, of the descriptor and all of its subdescriptors.

bNumDeviceCaps

The number of separate device capability descriptors in the binary object store.

