

- USBDriverKit
- IOUSBEndpointDescriptor
-  bmAttributes 

Instance Property

# bmAttributes

The attributes of the endpoint.

DriverKit 19.0+

``` source
uint8_t bmAttributes;
```

## Discussion

This field contains the transfer type, synchronization type, and usage type attributes for the endpoint. For a list of possible values, see Endpoint Attributes.

## See Also

### Accessing the Descriptor Properties

bLength

The length of the descriptor in bytes.

bDescriptorType

The type of the descriptor.

bEndpointAddress

The address of the endpoint.

wMaxPacketSize

The maximum packet size that the endpoint supports.

bInterval

The interval to use when polling the endpoint for data transfers, specified in frames or microframes depending on the device’s speed.

