

- Kernel
- Hardware Families
- USB
- Additional Specifications
-  IOUSBFindInterfaceRequest 

Type Alias

# IOUSBFindInterfaceRequest

The structure for finding an interface request.

macOS 10.0+

``` source
typedef struct IOUSBFindInterfaceRequest IOUSBFindInterfaceRequest;
```

## Topics

### Getting the Properties

bAlternateSetting

The alternative setting to find.

bInterfaceClass

The interface class to find.

bInterfaceProtocol

The interface protocol to find.

bInterfaceSubClass

The interface subclass to find.

## See Also

### Communication Requests

IOUSBBulkPipeReq

The structure that represents a bulk pipe request.

IOUSBFindEndpointRequest

The structure that represents an endoint request to locate.

