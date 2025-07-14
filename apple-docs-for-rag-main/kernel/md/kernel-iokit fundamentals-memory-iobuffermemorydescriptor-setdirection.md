

- Kernel
- IOKit Fundamentals
- Memory
- IOBufferMemoryDescriptor
-  setDirection 

Instance Method

# setDirection

Changes the direction associated with the buffer’s memory transfers.

macOS 10.11.4+

``` source
virtual void setDirection(IODirection direction);
```

## Parameters 

`direction`  

The new direction of transfers.

## See Also

### Configuring the Descriptor

- getCapacity

Returns the number of bytes the buffer is capable of holding.

- setLength

Sets the length of the data in the buffer.

