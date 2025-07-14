

- Kernel
- Deprecated Symbols
- IOUSBHostPipe
-  controlRequest Deprecated

Instance Method

# controlRequest

macOS 10.15.2–10.15.4Deprecated

``` source
virtual IOReturn controlRequest(IOService *forClient, StandardUSB::DeviceRequest & request, void *dataBuffer, uint32_t & bytesTransferred, uint32_t completionTimeoutMs);
```

