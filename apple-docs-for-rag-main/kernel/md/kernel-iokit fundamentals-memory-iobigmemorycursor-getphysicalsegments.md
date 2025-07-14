

- Kernel
- IOKit Fundamentals
- Memory
- IOBigMemoryCursor
-  getPhysicalSegments 

# getPhysicalSegments

Generates a big endian physical scatter/gather list given a memory descriptor.

``` source
virtual UInt32 getPhysicalSegments(
 IOMemoryDescriptor *descriptor, 
 IOByteCount fromPosition, 
 PhysicalSegment *segments, 
 UInt32 maxSegments, 
 UInt32 inMaxTransferSize = 0, 
 IOByteCount *transferSize = 0) 
```

## Parameters 

`descriptor`  

IOMemoryDescriptor that describes the data associated with an I/O request.

`fromPosition`  

Starting location of the I/O within a memory descriptor.

`segments`  

Pointer to an array of IOMemoryCursor::PhysicalSegments for the output physical scatter/gather list.

`maxSegments`  

Maximum number of segments that can be written to segments array.

`inMaxTransferSize`  

Maximum transfer size is limited to that many bytes, otherwise it defaults to the maximum transfer size specified when the memory cursor was initialized.

`transferSize`  

Pointer to an IOByteCount variable that can contain the total size of the transfer being described. Defaults to 0 indicating that no transfer size need be returned.

## Return Value

If the descriptor is exhausted of memory, a zero is returned, otherwise the number of segments that were filled in is returned.

## Overview

Generates a list of physical segments from the given memory descriptor, relative to the current position of the descriptor. Wraps IOMemoryCursor::genPhysicalSegments.

## See Also

### Miscellaneous

initWithSpecification

Primary initializer for the IOBigMemoryCursor class.

outputSegment

Outputs the given segment into the output segments array in big endian byte order.

withSpecification

Creates and initializes an IOBigMemoryCursor in one operation.

