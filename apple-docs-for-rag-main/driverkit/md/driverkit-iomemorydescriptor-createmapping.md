

- DriverKit
- IOMemoryDescriptor
-  CreateMapping 

Instance Method

# CreateMapping

Maps the contents of the memory block to the address space of the current process.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t CreateMapping(uint64_t options, uint64_t address, uint64_t offset, uint64_t length, uint64_t alignment, IOMemoryMap * * map);
```

## Parameters 

`options`  

The options to use when mapping the memory into this process. For a list of possible values, see Memory Map Options.

`address`  

The address in the current process’ memory space at which to place the memory block. Specify a value for this parameter only if you also specified the kIOMemoryMapFixedAddress option; otherwise, specify `0`.

`offset`  

The offset into the buffer to use as the first byte. Specify a value for this parameter only if you want to map from somewhere other than the first byte of the buffer; otherwise, specify `0`.

`length`  

The number of bytes accessible to the memory mapping. Specify `0` to map the entire buffer into memory, or specify a value that is less than the current length of the buffer.

`alignment`  

The byte alignment to use when mapping the memory into your process. Specify only 0 for this parameter.

`map`  

A variable in which to store the newly created IOMemoryMap object. The returned object has a retain count of 1. You are responsible for releasing this object when you are finished with it.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Use this method to map a memory buffer created by another process into the address space of the current process.

## See Also

### Mapping to the Caller’s Address Space

Memory Map Options

Options that describe how to configure a memory-mapped buffer.

