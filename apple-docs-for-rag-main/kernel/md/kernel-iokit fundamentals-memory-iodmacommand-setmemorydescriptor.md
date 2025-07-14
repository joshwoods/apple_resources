

- Kernel
- IOKit Fundamentals
- Memory
- IODMACommand
-  setMemoryDescriptor 

# setMemoryDescriptor

Sets and resets the DMACommand's current memory descriptor

``` source
virtual IOReturn setMemoryDescriptor(
 const IOMemoryDescriptor *mem, 
 bool autoPrepare = true); 
```

## Parameters 

`mem`  

A pointer to the current I/Os memory descriptor.

`autoPrepare`  

An optional boolean variable that will call the prepare() function automatically after the memory descriptor is processed. Defaults to true.

## Return Value

Returns kIOReturnSuccess, kIOReturnBusy if currently prepared, kIOReturnNoSpace if the length(mem) \>= Maximum Transfer Size or the error codes returned by prepare() (qv).

## Overview

The DMA command will configure itself based on the information that it finds in the memory descriptor. It looks for things like the direction of the memory descriptor and whether the current memory descriptor is already mapped into some IOMMU. As a programmer convenience it can also prepare the DMA command immediately. See prepare(). Note the IODMACommand is designed to used multiple times with a succession of memory descriptors, making the pooling of commands possible. It is an error though to attempt to reset a currently prepared() DMA command. Warning: This routine may block so never try to autoprepare an IODMACommand while in a gated context, i.e. one of the WorkLoops action call outs.

## See Also

### Configuring the Memory Descriptor

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

