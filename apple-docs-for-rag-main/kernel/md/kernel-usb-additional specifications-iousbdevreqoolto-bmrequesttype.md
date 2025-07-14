

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- Additional Specifications
- IOUSBDevReqOOLTO
-  bmRequestType 

Instance Property

# bmRequestType

The type of the request.

macOS 10.1+

``` source
UInt8 bmRequestType;
```

## See Also

### Getting the Properties

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

completionTimeout

The value of the completion timeout in milliseconds.

noDataTimeout

The value of the completion timeout in milliseconds if there’s no data.

