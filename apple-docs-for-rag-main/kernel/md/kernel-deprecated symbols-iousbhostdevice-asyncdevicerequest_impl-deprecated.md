

- Kernel
- Deprecated Symbols
- IOUSBHostDevice
-  AsyncDeviceRequest_Impl Deprecated

Instance Method

# AsyncDeviceRequest_Impl

macOS 10.15–10.15.4Deprecated

``` source
kern_return_t AsyncDeviceRequest_Impl(IOService *forClient, uint8_t bmRequestType, uint8_t bRequest, uint16_t wValue, uint16_t wIndex, uint16_t wLength, IOMemoryDescriptor *dataBuffer, OSAction *completion, uint32_t completionTimeoutMs);
```

