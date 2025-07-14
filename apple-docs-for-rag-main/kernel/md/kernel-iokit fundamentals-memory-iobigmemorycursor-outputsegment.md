

- Kernel
- IOKit Fundamentals
- Memory
- IOBigMemoryCursor
-  outputSegment 

# outputSegment

Outputs the given segment into the output segments array in big endian byte order.

``` source
static void outputSegment(
 PhysicalSegmentsegment, 
 void *segments, 
 UInt32segmentIndex); 
```

## Parameters 

`segment`  

The physical address and length that is next to be output.

`segments`  

Base of the output vector of DMA address length pairs.

`segmentIndex`  

Index to output 'segment' in the 'segments' array.

## See Also

### Miscellaneous

getPhysicalSegments

Generates a big endian physical scatter/gather list given a memory descriptor.

initWithSpecification

Primary initializer for the IOBigMemoryCursor class.

withSpecification

Creates and initializes an IOBigMemoryCursor in one operation.

