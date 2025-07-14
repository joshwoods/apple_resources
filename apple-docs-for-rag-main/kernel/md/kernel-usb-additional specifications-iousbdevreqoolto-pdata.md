

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- Additional Specifications
- IOUSBDevReqOOLTO
-  pData 

Instance Property

# pData

The pointer to the data for the request.

macOS 10.1+

``` source
void *pData;
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

wLenDone

The number of data bytes that the system actually transferred.

pipeRef

A reference to the USB pipe.

completionTimeout

The value of the completion timeout in milliseconds.

noDataTimeout

The value of the completion timeout in milliseconds if there’s no data.

