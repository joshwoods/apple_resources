

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- Additional Specifications
- IOUSBDevReqOOL
-  wValue 

Instance Property

# wValue

The 16-bit parameter for the request.

macOS 10.0+

``` source
UInt16 wValue;
```

## See Also

### Getting the Properties

bmRequestType

The type of the request.

bRequest

The request code.

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

