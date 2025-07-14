

- USBDriverKit
- IOUSBEndpointDescriptor
-  bLength 

Instance Property

# bLength

The length of the descriptor in bytes.

DriverKit 19.0+

``` source
uint8_t bLength;
```

## See Also

### Accessing the Descriptor Properties

bDescriptorType

The type of the descriptor.

bEndpointAddress

The address of the endpoint.

bmAttributes

The attributes of the endpoint.

wMaxPacketSize

The maximum packet size that the endpoint supports.

bInterval

The interval to use when polling the endpoint for data transfers, specified in frames or microframes depending on the device’s speed.

