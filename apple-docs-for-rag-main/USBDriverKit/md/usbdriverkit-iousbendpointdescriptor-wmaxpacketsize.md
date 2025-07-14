

- USBDriverKit
- IOUSBEndpointDescriptor
-  wMaxPacketSize 

Instance Property

# wMaxPacketSize

The maximum packet size that the endpoint supports.

DriverKit 19.0+

``` source
uint16_t wMaxPacketSize;
```

## See Also

### Accessing the Descriptor Properties

bLength

The length of the descriptor in bytes.

bDescriptorType

The type of the descriptor.

bEndpointAddress

The address of the endpoint.

bmAttributes

The attributes of the endpoint.

bInterval

The interval to use when polling the endpoint for data transfers, specified in frames or microframes depending on the device’s speed.

