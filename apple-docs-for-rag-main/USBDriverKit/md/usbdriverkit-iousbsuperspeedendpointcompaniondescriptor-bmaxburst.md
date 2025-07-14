

- USBDriverKit
- IOUSBSuperSpeedEndpointCompanionDescriptor
-  bMaxBurst 

Instance Property

# bMaxBurst

The maximum number of packets the endpoint can send or receive in one burst.

DriverKit 19.0+

``` source
uint8_t bMaxBurst;
```

## See Also

### Accessing the Descriptor Properties

bLength

The length of this descriptor in bytes.

bDescriptorType

The type of the descriptor.

bmAttributes

The attributes associated with the endpoint.

wBytesPerInterval

The total number of bytes this endpoint transfers during each service interval.

