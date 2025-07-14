

- Kernel
- IOKit Fundamentals
- Memory
- IOLittleMemoryCursor
-  withSpecification 

# withSpecification

Creates and initializes an IOLittleMemoryCursor in one operation.

``` source
static IOLittleMemoryCursor * withSpecification(
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

Factory function to create and initialize an IOLittleMemoryCursor in one operation. See also IOLittleMemoryCursor::initWithSpecification.

## See Also

### Miscellaneous

getPhysicalSegments

Generates a little endian physical scatter/gather list given a memory descriptor.

initWithSpecification

Primary initializer for the IOLittleMemoryCursor class.

outputSegment

Outputs the given segment into the output segments array in little endian byte order.

