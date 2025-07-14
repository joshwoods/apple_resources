

- Kernel
- IOKit Fundamentals
- Memory
- IOBigMemoryCursor
-  initWithSpecification 

# initWithSpecification

Primary initializer for the IOBigMemoryCursor class.

``` source
virtual bool initWithSpecification(
 IOPhysicalLength maxSegmentSize, 
 IOPhysicalLength maxTransferSize, 
 IOPhysicalLength alignment = 1); 
```

## Parameters 

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

getPhysicalSegments

Generates a big endian physical scatter/gather list given a memory descriptor.

outputSegment

Outputs the given segment into the output segments array in big endian byte order.

withSpecification

Creates and initializes an IOBigMemoryCursor in one operation.

