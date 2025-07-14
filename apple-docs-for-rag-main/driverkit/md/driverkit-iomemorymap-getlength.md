

- DriverKit
- IOMemoryMap
-  GetLength 

Instance Method

# GetLength

Returns the length of the memory block in bytes.

DriverKitiOSiPadOSmacOS

``` source
uint64_t GetLength();
```

## Return Value

The number of bytes in the memory block.

## Discussion

The length represents the number of bytes that are accessible to the current process.

## See Also

### Getting the Map Attributes

GetAddress

Returns the address of the memory block.

GetOffset

Returns the offset from the original start of the memory block.

