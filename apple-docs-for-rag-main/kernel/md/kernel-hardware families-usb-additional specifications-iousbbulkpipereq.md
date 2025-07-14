

- Kernel
- Hardware Families
- USB
- Additional Specifications
-  IOUSBBulkPipeReq 

Type Alias

# IOUSBBulkPipeReq

The structure that represents a bulk pipe request.

macOS 10.1+

``` source
typedef struct IOUSBBulkPipeReq IOUSBBulkPipeReq;
```

## Topics

### Getting the Properties

pipeRef

A reference to the USB pipe.

buf

A pointer to the request buffer.

size

The requested size of the pipe.

noDataTimeout

The timeout if no data is available.

completionTimeout

The completion timeout value.

## See Also

### Communication Requests

IOUSBFindInterfaceRequest

The structure for finding an interface request.

IOUSBFindEndpointRequest

The structure that represents an endoint request to locate.

