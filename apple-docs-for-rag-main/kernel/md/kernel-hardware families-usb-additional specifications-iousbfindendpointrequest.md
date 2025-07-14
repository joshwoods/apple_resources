

- Kernel
- Hardware Families
- USB
- Additional Specifications
-  IOUSBFindEndpointRequest 

Type Alias

# IOUSBFindEndpointRequest

The structure that represents an endoint request to locate.

macOS 10.0+

``` source
typedef struct IOUSBFindEndpointRequest IOUSBFindEndpointRequest;
```

## Topics

### Getting the Properties

type

The type of endpoint.

direction

The direction of the endpoint.

maxPacketSize

The maximum packet size of the endpoint.

interval

The polling interval for the endpoint in milliseconds.

## See Also

### Communication Requests

IOUSBFindInterfaceRequest

The structure for finding an interface request.

IOUSBBulkPipeReq

The structure that represents a bulk pipe request.

