

- AudioDriverKit
- IOUserAudioStream
-  SetIOMemoryDescriptor 

Instance Method

# SetIOMemoryDescriptor

Sets the memory descriptor the stream uses for I/O.

DriverKit 21.0+

``` source
kern_return_t SetIOMemoryDescriptor(IOMemoryDescriptor * in_io_memory_descriptor);
```

## See Also

### Working with Memory Descriptors

GetIOMemoryDescriptor

Gets the memory descriptor the stream uses for I/O.

