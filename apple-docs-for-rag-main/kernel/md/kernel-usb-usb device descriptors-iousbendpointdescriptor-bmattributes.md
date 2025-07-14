

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- USB Device Descriptors
- IOUSBEndpointDescriptor
-  bmAttributes 

Instance Property

# bmAttributes

The attributes of the endpoint.

macOS 10.0+

``` source
uint8_t bmAttributes;
```

## See Also

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bEndpointAddress

The address of the endpoint.

wMaxPacketSize

The maximum packet size that the endpoint supports.

bInterval

The interval to use when polling the endpoint for data transfers.

