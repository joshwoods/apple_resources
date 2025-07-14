

- Kernel
- IOKit Fundamentals
- Memory
- IOBufferMemoryDescriptor
-  appendBytes 

Instance Method

# appendBytes

Adds the specified data to the end of the memory buffer.

macOS 10.11.4+

``` source
virtual bool appendBytes(const void *bytes, vm_size_t withLength);
```

## Parameters 

`bytes`  

A pointer to the bytes to add.

`withLength`  

The number of bytes in the `bytes` parameter.

## Return Value

true if the bytes were appended successfully, or false if an error occurred.

