

- Kernel
- IOKit Fundamentals
- Memory
- IODMACommand
-  synchronize 

# synchronize

Bring IOMemoryDescriptor and IODMACommand buffers into sync.

``` source
virtual IOReturn synchronize(
 IOOptionBitsoptions); 
```

## Parameters 

`options`  

Specifies the direction of the copy: kIODirectionOut copy IOMemoryDesciptor memory to any IODMACommand buffers. By default this action takes place automatically at prepare(). kIODirectionIn copy any IODMACommand buffers back to the IOMemoryDescriptor. By default this action takes place automatically at complete(). kForceDoubleBuffer copy the entire prepared range to a new page aligned buffer.

## Return Value

kIOReturnNotReady if not prepared, kIOReturnBadArgument if invalid options are passed, kIOReturnSuccess otherwise.

## Overview

This method should not be called unless a prepare was previously issued. If needed a caller may synchronize any IODMACommand buffers with the original IOMemoryDescriptor buffers.

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

complete

Complete processing of DMA mappings after an I/O transfer is finished.

- complete

Complete processing of DMA mappings after an I/O transfer is finished.

- synchronize

Bring IOMemoryDescriptor and IODMACommand buffers into sync.

