

- Kernel
- Hardware Families
- USB
- Additional Specifications
-  IOUSBDevRequest 

Type Alias

# IOUSBDevRequest

A structure that defines a standard device request.

macOS 10.0+

``` source
typedef struct IOUSBDevRequest IOUSBDevRequest;
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

The number of data bytes that the system actually transferred.

## See Also

### Device Requests

IOUSBDevReqOOL

An internal structure to pass parameters between IOUSBLib and UserClient.

IOUSBDevReqOOLTO

An internal structure to pass parameters between IOUSBLib and UserClient.

IOUSBDevRequestTO

A structure that defines a standard device request with timeout.

IOUSBDeviceRequest

A structure that defines a standard device request.

IOUSBDeviceRequestPtr

A pointer to a structure that defines a standard device request.

IOUSBDeviceRequestSetSELData

The structure for receiving system exit latency values.

