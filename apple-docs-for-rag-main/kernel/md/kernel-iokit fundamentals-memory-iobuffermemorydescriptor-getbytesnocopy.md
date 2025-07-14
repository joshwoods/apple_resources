

- Kernel
- IOKit Fundamentals
- Memory
- IOBufferMemoryDescriptor
-  getBytesNoCopy 

Instance Method

# getBytesNoCopy

Returns the virtual address of an offset into the memory buffer.

macOS 10.15.2+

``` source
virtual void * getBytesNoCopy(vm_size_t start, vm_size_t withLength);
```

## Parameters 

`start`  

The offset from the beginning of the memory buffer.

`withLength`  

The number of bytes you want.

## Return Value

The address at the specified offset into the bufer, or `NULL` if the offset and length yield an invalid address range.

## See Also

### Getting the Buffer Contents

- getBytesNoCopy

Returns the virtual address of the beginning of the memory buffer.

