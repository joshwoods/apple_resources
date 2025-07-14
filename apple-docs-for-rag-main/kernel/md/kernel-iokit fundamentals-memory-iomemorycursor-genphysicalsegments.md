

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryCursor
-  genPhysicalSegments 

# genPhysicalSegments

Generates a physical scatter/gather list given a memory descriptor.

``` source
virtual UInt32 genPhysicalSegments( 
 IOMemoryDescriptor *descriptor, 
 IOByteCount fromPosition, 
 void *segments, 
 UInt32 maxSegments, 
 UInt32 maxTransferSize = 0, 
 IOByteCount *transferSize = 0); 
```

## Parameters 

`descriptor`  

IOMemoryDescriptor that describes the data associated with an I/O request.

`fromPosition`  

Starting location of the I/O within a memory descriptor.

`segments`  

Void pointer to base of output physical scatter/gather list. Always passed directly onto the SegmentFunction without interpretation by the cursor.

`maxSegments`  

Maximum number of segments that can be written to segments array.

`maxTransferSize`  

Maximum transfer size is limited to that many bytes, otherwise it defaults to the maximum transfer size specified when the memory cursor was initialized.

`transferSize`  

Pointer to an IOByteCount variable that can contain the total size of the transfer being described. Defaults to 0 indicating that no transfer size need be returned.

## Return Value

If the descriptor is exhausted of memory, a zero is returned, otherwise the number of segments that were filled in is returned.

## Overview

Generates a list of physical segments from the given memory descriptor, relative to the current position of the descriptor.

## See Also

### Miscellaneous

initWithSpecification

Primary initializer for the IOMemoryCursor class.

withSpecification

Creates and initializes an IOMemoryCursor in one operation.

