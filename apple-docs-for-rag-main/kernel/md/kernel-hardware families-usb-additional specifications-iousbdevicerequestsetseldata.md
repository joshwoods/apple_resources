

- Kernel
- Hardware Families
- USB
- Additional Specifications
-  IOUSBDeviceRequestSetSELData 

Type Alias

# IOUSBDeviceRequestSetSELData

The structure for receiving system exit latency values.

macOS 10.15+

``` source
typedef struct IOUSBDeviceRequestSetSELData IOUSBDeviceRequestSetSELData;
```

## Discussion

For information about the `Set SEL` request type, see USB 3.2, 9.4.12.

## Topics

### Instance Properties

u1Pel

u1Sel

u2Pel

u2Sel

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

IOUSBDeviceRequest

A structure that defines a standard device request.

IOUSBDeviceRequestPtr

A pointer to a structure that defines a standard device request.

