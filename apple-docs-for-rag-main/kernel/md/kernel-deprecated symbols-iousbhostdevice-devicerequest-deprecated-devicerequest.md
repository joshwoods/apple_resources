

- Kernel
- Deprecated Symbols
- IOUSBHostDevice
-  deviceRequest Deprecated

Instance Method

# deviceRequest

macOS 10.15.2–10.15.4Deprecated

``` source
virtual IOReturn deviceRequest(IOService *forClient, StandardUSB::DeviceRequest & request, void *rawBuffer, IOMemoryDescriptor *descriptorBuffer, uint32_t & bytesTransferred, IOUSBHostCompletion *completion, uint32_t completionTimeoutMs);
```

