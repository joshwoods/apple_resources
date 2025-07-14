

- Kernel
- Hardware Families
- USB
- Additional Specifications
-  IOUSBDeviceRequest 

Type Alias

# IOUSBDeviceRequest

A structure that defines a standard device request.

macOS 10.15+

``` source
typedef struct IOUSBDeviceRequest IOUSBDeviceRequest;
```

## Discussion

For information about device requests, see USB 3.2, 9.3.

## Topics

### Instance Properties

bRequest

bmRequestType

wIndex

wLength

wValue

## See Also

### Device Requests

IOUSBDevReqOOL

An internal structure to pass parameters between IOUSBLib and UserClient.

IOUSBDevReqOOLTO

An internal structure to pass parameters between IOUSBLib and UserClient.

IOUSBDevRequest

A structure that defines a standard device request.

IOUSBDevRequestTO

A structure that defines a standard device request with timeout.

IOUSBDeviceRequestPtr

A pointer to a structure that defines a standard device request.

IOUSBDeviceRequestSetSELData

The structure for receiving system exit latency values.

