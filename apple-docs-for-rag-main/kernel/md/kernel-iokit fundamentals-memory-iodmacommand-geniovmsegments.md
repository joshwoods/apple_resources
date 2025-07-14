

- Kernel
- IOKit Fundamentals
- Memory
- IODMACommand
-  genIOVMSegments 

# genIOVMSegments

Generates a physical scatter/gather for the current DMA command

``` source
virtual IOReturn genIOVMSegments(
 UInt64 *offset, 
 void *segments, 
 UInt32 *numSegments); 
```

## Parameters 

`offset`  

input/output parameter, defines the starting and ending offset in the memory descriptor, relative to any offset passed to the prepare() method.

`segments`  

Void pointer to base of output physical scatter/gather list. Always passed directly onto the SegmentFunction.

`numSegments`  

Input/output parameter Number of segments that can fit in the segment array and returns number of segments generated.

## Return Value

kIOReturnSuccess on success, kIOReturnOverrun if the memory descriptor is exhausted, kIOReturnMessageTooLarge if the output segment function's address bits has insufficient resolution for a segment, kIOReturnNotReady if the DMA command has not be prepared, kIOReturnBadArgument if the DMA command doesn't have a memory descriptor yet or some of the parameters are NULL and kIOReturnNotReady if the DMA command is not prepared.

## Overview

Generates a list of physical segments from the given memory descriptor, relative to the current position of the descriptor. The constraints that are set during initialisation will be respected. This function maintains the state across multiple calls for efficiency. However the state is discarded if the new offset is not the expected one.

## See Also

### Configuring the Memory Descriptor

setMemoryDescriptor

Sets and resets the DMACommand's current memory descriptor

- setMemoryDescriptor

Sets and resets the DMACommand's current memory descriptor

clearMemoryDescriptor

Clears the DMACommand's current memory descriptor

- clearMemoryDescriptor

Clears the DMACommand's current memory descriptor

getMemoryDescriptor

Get the current memory descriptor

- getMemoryDescriptor

Get the current memory descriptor

- getIOMemoryDescriptor

getPreparedOffsetAndLength

Returns the offset and length into the target IOMemoryDescriptor of a prepared IODDMACommand.

- getPreparedOffsetAndLength

Returns the offset and length into the target IOMemoryDescriptor of a prepared IODDMACommand.

- genIOVMSegments

Generates a physical scatter/gather for the current DMA command

gen32IOVMSegments

Helper function for a type checked call to genIOVMSegments(qv), for use with an IODMACommand set up with the output function kIODMACommandOutputHost32, kIODMACommandOutputBig32, or kIODMACommandOutputLittle32. If the output function of the IODMACommand is not a 32 bit function, results will be incorrect.

- gen32IOVMSegments

gen64IOVMSegments

Helper function for a type checked call to genIOVMSegments(qv), for use with an IODMACommand set up with the output function kIODMACommandOutputHost64, kIODMACommandOutputBig64, or kIODMACommandOutputLittle64. If the output function of the IODMACommand is not a 64 bit function, results will be incorrect.

- gen64IOVMSegments

- createCopyBuffer

