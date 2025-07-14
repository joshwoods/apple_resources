

- DriverKit
- IOBufferMemoryDescriptor
-  Create 

Static Method

# Create

Creates a new memory buffer descriptor object in the current process space.

DriverKitiOSiPadOSmacOS

``` source
static kern_return_t Create(uint64_t options, uint64_t capacity, uint64_t alignment, IOBufferMemoryDescriptor * * memory);
```

## Parameters 

`options`  

The direction in which buffer data moves, relative to your process. For example, specify kIOMemoryDirectionIn if your driver only reads from the buffer. For a list of possible values, see `Memory Buffer Options`.

`capacity`  

The maximum number of bytes to allocate for the memory buffer. The buffer’s initial length is set to the value in this parameter. You can change the length later by calling the SetLength method.

`alignment`  

The minimum required alignment of the buffer in bytes. For example, specify 256 to align the buffer on an address where bits 0 to 7 are `0`. Specify `0` if you don’t require a specific alignment.

`memory`  

A variable in which to store the newly created buffer memory descriptor.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Creating a Memory Buffer

init

Initializes the buffer memory descriptor object.

free

Performs any final cleanup for the memory buffer descriptor object.

