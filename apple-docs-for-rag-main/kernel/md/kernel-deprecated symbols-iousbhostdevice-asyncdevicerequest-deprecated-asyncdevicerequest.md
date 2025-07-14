

- Kernel
- Deprecated Symbols
- IOUSBHostDevice
-  AsyncDeviceRequest Deprecated

Instance Method

# AsyncDeviceRequest

macOS 10.15–10.15.4Deprecated

``` source
kern_return_t AsyncDeviceRequest(IOService *forClient, uint8_t bmRequestType, uint8_t bRequest, uint16_t wValue, uint16_t wIndex, uint16_t wLength, IOMemoryDescriptor *dataBuffer, OSAction *completion, uint32_t completionTimeoutMs, OSDispatchMethod supermethod);
```

