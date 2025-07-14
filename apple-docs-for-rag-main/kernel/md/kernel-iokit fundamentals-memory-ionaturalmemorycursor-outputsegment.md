

- Kernel
- IOKit Fundamentals
- Memory
- IONaturalMemoryCursor
-  outputSegment 

# outputSegment

Outputs the given segment into the output segments array in natural byte order.

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

Generates a CPU natural physical scatter/gather list given a memory descriptor.

initWithSpecification

Primary initializer for the IONaturalMemoryCursor class.

withSpecification

Creates and initializes an IONaturalMemoryCursor in one operation.

