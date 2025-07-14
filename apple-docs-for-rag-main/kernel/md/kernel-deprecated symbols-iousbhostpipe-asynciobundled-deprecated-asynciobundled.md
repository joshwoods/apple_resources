

- Kernel
- Deprecated Symbols
- IOUSBHostPipe
-  AsyncIOBundled Deprecated

Instance Method

# AsyncIOBundled

macOS 10.15–10.15.4Deprecated

``` source
kern_return_t AsyncIOBundled(uint32_t ioTransferIndex, uint32_t ioTransferCount, uint32_t *ioTransferAcceptedCount, const unsigned int *dataBufferLengthArray, int dataBufferLengthArrayCount, OSAction *completion, uint32_t completionTimeoutMs, OSDispatchMethod supermethod);
```

