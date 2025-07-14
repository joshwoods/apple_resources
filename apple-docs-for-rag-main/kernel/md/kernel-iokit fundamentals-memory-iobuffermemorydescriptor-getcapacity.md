

- Kernel
- IOKit Fundamentals
- Memory
- IOBufferMemoryDescriptor
-  getCapacity 

Instance Method

# getCapacity

Returns the number of bytes the buffer is capable of holding.

macOS 10.11.4+

``` source
virtual vm_size_t getCapacity(void);
```

## See Also

### Configuring the Descriptor

- setDirection

Changes the direction associated with the buffer’s memory transfers.

- setLength

Sets the length of the data in the buffer.

