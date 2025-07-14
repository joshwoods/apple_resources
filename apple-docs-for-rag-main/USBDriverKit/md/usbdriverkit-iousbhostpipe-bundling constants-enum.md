

- USBDriverKit
- IOUSBHostPipe
-  Bundling Constants 

API Collection

# Bundling Constants

Constants associated with bulk I/O transfers.

## Topics

### Bundling Options

kIOUSBHostPipeBundlingMax

The maximum number of elements to transfer in one bundled I/O call.

## See Also

### Interacting with Descriptor Rings

kern_return_t CreateMemoryDescriptorRing(uint32_t size);

kern_return_t SetMemoryDescriptor(IOMemoryDescriptor * memoryDescriptor, uint32_t index);

AsyncIOBundled

Enqueues a contiguous group of requests from the descriptor ring.

CompleteAsyncIOBundled

Handles the completion of an asynchronous bundled transfer.

