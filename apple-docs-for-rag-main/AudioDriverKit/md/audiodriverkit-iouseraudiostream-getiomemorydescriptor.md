

- AudioDriverKit
- IOUserAudioStream
-  GetIOMemoryDescriptor 

Instance Method

# GetIOMemoryDescriptor

Gets the memory descriptor the stream uses for I/O.

DriverKit 21.0+

``` source
OSSharedPtr GetIOMemoryDescriptor();
```

## Discussion

This is the value provided to the stream’s initializer, or updated later by a call to SetIOMemoryDescriptor.

## See Also

### Working with Memory Descriptors

SetIOMemoryDescriptor

Sets the memory descriptor the stream uses for I/O.

