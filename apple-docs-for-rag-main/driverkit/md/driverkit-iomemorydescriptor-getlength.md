

- DriverKit
- IOMemoryDescriptor
-  GetLength 

Instance Method

# GetLength

Returns the length of the memory block represented by this object.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t GetLength(uint64_t * returnLength);
```

## Parameters 

`returnLength`  

A variable in which to put the length of the current memory block.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

This method returns the effective size of the memory block, which might be less than the block’s total capacity.

## See Also

### Related Documentation

SetLength

Changes the length of the memory buffer.

