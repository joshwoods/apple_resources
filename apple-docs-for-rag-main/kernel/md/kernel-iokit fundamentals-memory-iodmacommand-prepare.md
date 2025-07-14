

- Kernel
- IOKit Fundamentals
- Memory
- IODMACommand
-  prepare 

# prepare

Prepare the memory for an I/O transfer.

``` source
virtual IOReturn prepare(
 UInt64 offset = 0,
 UInt64 length = 0,
 bool flushCache = true,
 bool synchronize = true); 
```

## Parameters 

`offset`  

defines the starting offset in the memory descriptor the DMA command will operate on. genIOVMSegments will produce its results based on the offset and length passed to the prepare method.

`length`  

defines the ending position in the memory descriptor the DMA command will operate on. genIOVMSegments will produce its results based on the offset and length passed to the prepare method.

`flushCache`  

Flush the caches for the memory descriptor and make certain that the memory cycles are complete. Defaults to true for kNonCoherent and is ignored by the other types.

`synchronize`  

Copy any buffered data back from the target IOMemoryDescriptor. Defaults to true, if synchronize() is being used to explicitly copy data, passing false may avoid an unneeded copy.

## Return Value

An IOReturn code.

## Overview

Allocate the mapping resources neccessary for this transfer, specifying a sub range of the IOMemoryDescriptor that will be the target of the I/O. The complete() method frees these resources. Data may be copied to buffers for kIODirectionOut memory descriptors, depending on hardware mapping resource availabilty or alignment restrictions. It should be noted that the this function may block and should only be called on the clients context, i.e never call this routine while gated; also the call itself is not thread safe though this should be an issue as each IODMACommand is independant.

## See Also

### Preparing the Transfer Operation

- prepare

Prepare the memory for an I/O transfer.

prepareWithSpecification

Prepare the memory for an I/O transfer with a new specification.

- prepareWithSpecification

Prepare the memory for an I/O transfer with a new specification.

- prepareWithSpecification

Prepare the memory for an I/O transfer with a new specification.

complete

Complete processing of DMA mappings after an I/O transfer is finished.

- complete

Complete processing of DMA mappings after an I/O transfer is finished.

synchronize

Bring IOMemoryDescriptor and IODMACommand buffers into sync.

- synchronize

Bring IOMemoryDescriptor and IODMACommand buffers into sync.

