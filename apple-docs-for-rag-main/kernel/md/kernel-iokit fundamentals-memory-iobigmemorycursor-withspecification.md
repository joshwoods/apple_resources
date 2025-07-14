

- Kernel
- IOKit Fundamentals
- Memory
- IOBigMemoryCursor
-  withSpecification 

# withSpecification

Creates and initializes an IOBigMemoryCursor in one operation.

``` source
static IOBigMemoryCursor * withSpecification(
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

Returns a new memory cursor if successfully created and initialized, 0 otherwise.

## Overview

Factory function to create and initialize an IOBigMemoryCursor in one operation. See also IOBigMemoryCursor::initWithSpecification.

## See Also

### Miscellaneous

getPhysicalSegments

Generates a big endian physical scatter/gather list given a memory descriptor.

initWithSpecification

Primary initializer for the IOBigMemoryCursor class.

outputSegment

Outputs the given segment into the output segments array in big endian byte order.

