

- Kernel
- IOKit Fundamentals
- Memory
- IODMACommand
-  complete 

# complete

Complete processing of DMA mappings after an I/O transfer is finished.

``` source
virtual IOReturn complete(
 bool invalidateCache = true,
 bool synchronize = true); 
```

## Parameters 

`invalidCache`  

Invalidate the caches for the memory descriptor. Defaults to true for kNonCoherent and is ignored by the other types.

`synchronize`  

Copy any buffered data back to the target IOMemoryDescriptor. Defaults to true, if synchronize() is being used to explicitly copy data, passing false may avoid an unneeded copy.

## Return Value

kIOReturnNotReady if not prepared, kIOReturnSuccess otherwise.

## Overview

This method should not be called unless a prepare was previously issued; the prepare() and complete() must occur in pairs, before and after an I/O transfer

## See Also

### Preparing the Transfer Operation

prepare

Prepare the memory for an I/O transfer.

- prepare

Prepare the memory for an I/O transfer.

prepareWithSpecification

Prepare the memory for an I/O transfer with a new specification.

- prepareWithSpecification

Prepare the memory for an I/O transfer with a new specification.

- prepareWithSpecification

Prepare the memory for an I/O transfer with a new specification.

- complete

Complete processing of DMA mappings after an I/O transfer is finished.

synchronize

Bring IOMemoryDescriptor and IODMACommand buffers into sync.

- synchronize

Bring IOMemoryDescriptor and IODMACommand buffers into sync.

