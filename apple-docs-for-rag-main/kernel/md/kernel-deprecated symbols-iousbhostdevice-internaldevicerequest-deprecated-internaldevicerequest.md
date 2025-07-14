

- Kernel
- Deprecated Symbols
- IOUSBHostDevice
-  internalDeviceRequest Deprecated

Instance Method

# internalDeviceRequest

macOS 10.11.4–10.15.4Deprecated

``` source
virtual IOReturn internalDeviceRequest(IOService *forClient, StandardUSB::DeviceRequest & request, void *rawBuffer, IOMemoryDescriptor *descriptorBuffer, uint32_t & bytesTransferred, IOUSBHostCompletion *completion, uint32_t completionTimeoutMs);
```

