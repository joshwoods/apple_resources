

- DriverKit
- IOUserClient
-  CopyClientMemoryForType 

Instance Method

# CopyClientMemoryForType

Return an IOMemoryDescriptor to be mapped into the client task.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t CopyClientMemoryForType(uint64_t type, uint64_t * options, IOMemoryDescriptor * * memory);
```

## Parameters 

`type`  

Type parameter IOConnectMapMemory()/UnmapMemory().

`options`  

Set kIOUserClientMemoryReadOnly for memory to be mapped read only in the client.

`memory`  

An instance of IOMemoryDescriptor on success. One reference will be consumed by the caller of this method.

## Return Value

kIOReturnSuccess on success. See IOReturn.h for error codes.

## Discussion

IOConnectMapMemory()/UnmapMemory() will result in a call to this method to obtain an IOMemoryDescriptor instance for shared memory. For a given IOUserClient instance, calling CopyClientMemoryForType() with a given type, should return the same IOMemoryDescriptor instance.

## See Also

### Mapping to the Client’s Memory Space

Copy Client Memory Options

