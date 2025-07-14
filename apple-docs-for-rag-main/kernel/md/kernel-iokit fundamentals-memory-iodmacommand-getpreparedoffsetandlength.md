

- Kernel
- IOKit Fundamentals
- Memory
- IODMACommand
-  getPreparedOffsetAndLength 

# getPreparedOffsetAndLength

Returns the offset and length into the target IOMemoryDescriptor of a prepared IODDMACommand.

``` source
virtual IOReturn getPreparedOffsetAndLength(
 UInt64 *offset,
 UInt64 *length); 
```

## Parameters 

`offset`  

returns the starting offset in the memory descriptor the DMA command was prepared with. Pass NULL for don't care.

`length`  

returns the length in the memory descriptor the DMA command was prepared with. Pass NULL for don't care.

## Return Value

An IOReturn code. kIOReturnNotReady if the IODMACommand is not prepared.

## Overview

If successfully prepared, returns the offset and length into the IOMemoryDescriptor. Will fail for an unprepared IODMACommand.

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

- getPreparedOffsetAndLength

Returns the offset and length into the target IOMemoryDescriptor of a prepared IODDMACommand.

genIOVMSegments

Generates a physical scatter/gather for the current DMA command

- genIOVMSegments

Generates a physical scatter/gather for the current DMA command

gen32IOVMSegments

Helper function for a type checked call to genIOVMSegments(qv), for use with an IODMACommand set up with the output function kIODMACommandOutputHost32, kIODMACommandOutputBig32, or kIODMACommandOutputLittle32. If the output function of the IODMACommand is not a 32 bit function, results will be incorrect.

- gen32IOVMSegments

gen64IOVMSegments

Helper function for a type checked call to genIOVMSegments(qv), for use with an IODMACommand set up with the output function kIODMACommandOutputHost64, kIODMACommandOutputBig64, or kIODMACommandOutputLittle64. If the output function of the IODMACommand is not a 64 bit function, results will be incorrect.

- gen64IOVMSegments

- createCopyBuffer

