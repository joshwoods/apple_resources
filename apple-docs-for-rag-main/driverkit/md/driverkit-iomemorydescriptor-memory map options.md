

- DriverKit
- IOMemoryDescriptor
-  Memory Map Options 

API Collection

# Memory Map Options

Options that describe how to configure a memory-mapped buffer.

## Topics

### Options

kIOMemoryMapFixedAddress

The memory maps to a specific address.

kIOMemoryMapReadOnly

The memory maps as read-only.

kIOMemoryMapCacheModeDefault

The memory maps using the default cache mode.

kIOMemoryMapCacheModeInhibit

The memory maps using the inhibited cache mode.

kIOMemoryMapCacheModeCopyback

The memory maps using the copy-back cache mode.

kIOMemoryMapCacheModeWriteThrough

The memory maps using the write-through cache mode.

## See Also

### Mapping to the Caller’s Address Space

CreateMapping

Maps the contents of the memory block to the address space of the current process.

