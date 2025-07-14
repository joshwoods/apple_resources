

- USBDriverKit
- IOUSBSuperSpeedEndpointCompanionDescriptor
-  wBytesPerInterval 

Instance Property

# wBytesPerInterval

The total number of bytes this endpoint transfers during each service interval.

DriverKit 19.0+

``` source
uint16_t wBytesPerInterval;
```

## See Also

### Accessing the Descriptor Properties

bLength

The length of this descriptor in bytes.

bDescriptorType

The type of the descriptor.

bMaxBurst

The maximum number of packets the endpoint can send or receive in one burst.

bmAttributes

The attributes associated with the endpoint.

