

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryCursor
-  initWithSpecification 

# initWithSpecification

Primary initializer for the IOMemoryCursor class.

``` source
virtual bool initWithSpecification(
 SegmentFunction outSegFunc, 
 IOPhysicalLength maxSegmentSize = 0, 
 IOPhysicalLength maxTransferSize = 0, 
 IOPhysicalLength alignment = 1); 
```

## Parameters 

`outSegFunc`  

SegmentFunction to call to output one physical segment.

`maxSegmentSize`  

Maximum allowable size for one segment. Defaults to 0.

`maxTransferSize`  

Maximum size of an entire transfer. Defaults to 0 indicating no maximum.

`alignment`  

Alignment restrictions on output physical addresses. Not currently implemented. Defaults to single byte alignment.

## Return Value

Returns true if the inherited classes and this instance initialize successfully.

## See Also

### Miscellaneous

genPhysicalSegments

Generates a physical scatter/gather list given a memory descriptor.

withSpecification

Creates and initializes an IOMemoryCursor in one operation.

