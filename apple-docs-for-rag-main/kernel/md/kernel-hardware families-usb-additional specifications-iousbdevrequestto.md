

- Kernel
- Hardware Families
- USB
- Additional Specifications
-  IOUSBDevRequestTO 

Type Alias

# IOUSBDevRequestTO

A structure that defines a standard device request with timeout.

macOS 10.1+

``` source
typedef struct IOUSBDevRequestTO IOUSBDevRequestTO;
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

completionTimeout

The value of the completion timeout in milliseconds.

noDataTimeout

The value of the completion timeout in milliseconds if there’s no data.

## See Also

### Device Requests

IOUSBDevReqOOL

An internal structure to pass parameters between IOUSBLib and UserClient.

IOUSBDevReqOOLTO

An internal structure to pass parameters between IOUSBLib and UserClient.

IOUSBDevRequest

A structure that defines a standard device request.

IOUSBDeviceRequest

A structure that defines a standard device request.

IOUSBDeviceRequestPtr

A pointer to a structure that defines a standard device request.

IOUSBDeviceRequestSetSELData

The structure for receiving system exit latency values.

