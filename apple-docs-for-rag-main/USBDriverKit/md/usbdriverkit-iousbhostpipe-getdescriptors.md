

- USBDriverKit
- IOUSBHostPipe
-  GetDescriptors 

Instance Method

# GetDescriptors

Retrieves the endpoint descriptors associated with this pipe.

DriverKit 19.0+

``` source
kern_return_t GetDescriptors(IOUSBStandardEndpointDescriptors * descriptors, IOUSBGetEndpointDescriptorOptions type);
```

## Parameters 

`descriptors`  

A pointer to a variable. On output, this variable contains the endpoint descriptors for the pipe.

`type`  

The options indicating which descriptors to retrieve. For a list of possible values, see IOUSBGetEndpointDescriptorOptions.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Getting the Endpoint Descriptors

IOUSBStandardEndpointDescriptors

Encapsulates the descriptors for a single endpoint.

IOUSBGetEndpointDescriptorOptions

Options for fetching the endpoint descriptors of a pipe.

