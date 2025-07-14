

- USBDriverKit
- IOUSBHostPipe
-  AdjustPipe 

Instance Method

# AdjustPipe

Adjusts the behavior of periodic endpoints to consume a different amount of bus bandwidth.

DriverKit 19.0+

``` source
kern_return_t AdjustPipe(const IOUSBStandardEndpointDescriptors * descriptors);
```

## Parameters 

`descriptors`  

A pointer to a descriptor’s structure describing the new endpoint policy. Copy the original endpoint descriptors and modify to adjust maximum packet size, burst, and interval values.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Periodic (interrupt and isochronous) endpoints reserve bus bandwidth when they’re created. This reserved bandwidth takes into account the maximum packet size, burst size, and endpoint service interval. If you know the endpoint won’t use all of its allocated bandwidth, you can call the `AdjustPipe` method to reduce the bandwidth reserved for the endpoint.

## See Also

### Adjusting the Pipe’s Status

ClearStall

Clears the halt condition of the pipe.

