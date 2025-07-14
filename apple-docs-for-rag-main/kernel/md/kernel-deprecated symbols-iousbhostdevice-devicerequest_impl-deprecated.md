

- Kernel
- Deprecated Symbols
- IOUSBHostDevice
-  DeviceRequest_Impl Deprecated

Instance Method

# DeviceRequest_Impl

macOS 10.15–10.15.4Deprecated

``` source
kern_return_t DeviceRequest_Impl(IOService *forClient, uint8_t bmRequestType, uint8_t bRequest, uint16_t wValue, uint16_t wIndex, uint16_t wLength, IOMemoryDescriptor *dataBuffer, uint16_t *bytesTransferred, uint32_t completionTimeoutMs);
```

