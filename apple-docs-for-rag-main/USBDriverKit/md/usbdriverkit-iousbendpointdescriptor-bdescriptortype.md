

- USBDriverKit
- IOUSBEndpointDescriptor
-  bDescriptorType 

Instance Property

# bDescriptorType

The type of the descriptor.

DriverKit 19.0+

``` source
uint8_t bDescriptorType;
```

## See Also

### Accessing the Descriptor Properties

bLength

The length of the descriptor in bytes.

bEndpointAddress

The address of the endpoint.

bmAttributes

The attributes of the endpoint.

wMaxPacketSize

The maximum packet size that the endpoint supports.

bInterval

The interval to use when polling the endpoint for data transfers, specified in frames or microframes depending on the device’s speed.

