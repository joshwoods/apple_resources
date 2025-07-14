

- Kernel
- Hardware Families
- USB
- Additional Specifications
-  IOUSBDevReqOOL 

Type Alias

# IOUSBDevReqOOL

An internal structure to pass parameters between IOUSBLib and UserClient.

macOS 10.0+

``` source
typedef struct IOUSBDevReqOOL IOUSBDevReqOOL;
```

## Topics

### Getting the Properties

bmRequestType

The type of the request.

bRequest

The request code.

wValue

The 16-bit parameter for the request.

wIndex

The 16-bit parameter for the request.

wLength

The length of the data part of the request.

pData

The pointer to the data for the request.

wLenDone

The number of data bytes that the system actually transferred.

pipeRef

A reference to the USB pipe.

## See Also

### Device Requests

IOUSBDevReqOOLTO

An internal structure to pass parameters between IOUSBLib and UserClient.

IOUSBDevRequest

A structure that defines a standard device request.

IOUSBDevRequestTO

A structure that defines a standard device request with timeout.

IOUSBDeviceRequest

A structure that defines a standard device request.

IOUSBDeviceRequestPtr

A pointer to a structure that defines a standard device request.

IOUSBDeviceRequestSetSELData

The structure for receiving system exit latency values.

