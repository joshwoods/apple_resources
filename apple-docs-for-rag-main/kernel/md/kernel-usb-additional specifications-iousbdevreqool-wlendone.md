

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- Additional Specifications
- IOUSBDevReqOOL
-  wLenDone 

Instance Property

# wLenDone

The number of data bytes that the system actually transferred.

macOS 10.0+

``` source
UInt32 wLenDone;
```

## See Also

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

pipeRef

A reference to the USB pipe.

