

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- USB Device Descriptors
- IOUSBEndpointDescriptor
-  bInterval 

Instance Property

# bInterval

The interval to use when polling the endpoint for data transfers.

macOS 10.0+

``` source
uint8_t bInterval;
```

## Discussion

Specify the value in frames or microframes, depending on the device’s speed.

## See Also

### Getting the Properties

bLength

The size of the descriptor.

bDescriptorType

The type of the descriptor.

bEndpointAddress

The address of the endpoint.

bmAttributes

The attributes of the endpoint.

wMaxPacketSize

The maximum packet size that the endpoint supports.

