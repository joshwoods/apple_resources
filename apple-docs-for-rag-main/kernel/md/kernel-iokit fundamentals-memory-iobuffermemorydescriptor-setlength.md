

- Kernel
- IOKit Fundamentals
- Memory
- IOBufferMemoryDescriptor
-  setLength 

Instance Method

# setLength

Sets the length of the data in the buffer.

macOS 10.11.4+

``` source
virtual void setLength(vm_size_t length);
```

## Parameters 

`length`  

The new length of the buffer. This value must be less than or equal to the capacity of the buffer.

## Discussion

At creation time, the system sets the buffer’s length to its capacity. Use this method to indicate that there are fewer bytes in the buffer than the total overall capacity. For example, you might set the length to minimize the amount of data you transfer. This method doesn’t change the total capacity of the buffer. Changing the length of a buffer allows you to reuse a buffer for multiple transfers of different lengths.

## See Also

### Configuring the Descriptor

- getCapacity

Returns the number of bytes the buffer is capable of holding.

- setDirection

Changes the direction associated with the buffer’s memory transfers.

