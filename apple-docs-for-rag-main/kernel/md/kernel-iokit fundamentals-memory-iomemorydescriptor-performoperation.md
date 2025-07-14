

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  performOperation 

# performOperation

Perform an operation on the memory descriptor's memory.

``` source
virtual IOReturn performOperation(
 IOOptionBitsoptions, 
 IOByteCountoffset,
 IOByteCountlength ); 
```

## Parameters 

`options`  

The operation to perform on the memory:

kIOMemoryIncoherentIOFlush - pass this option to store to memory and flush any data in the processor cache for the memory range, with synchronization to ensure the data has passed through all levels of processor cache. It may not be supported on all architectures. This type of flush may be used for non-coherent I/O such as AGP - it is NOT required for PCI coherent operations. The memory descriptor must have been previously prepared.

kIOMemoryIncoherentIOStore - pass this option to store to memory any data in the processor cache for the memory range, with synchronization to ensure the data has passed through all levels of processor cache. It may not be supported on all architectures. This type of flush may be used for non-coherent I/O such as AGP - it is NOT required for PCI coherent operations. The memory descriptor must have been previously prepared.

`offset`  

A byte offset into the memory descriptor's memory.

`length`  

The length of the data range.

## Return Value

An IOReturn code.

## Overview

This method performs some operation on a range of the memory descriptor's memory. When a memory descriptor's memory is not mapped, it should be more efficient to use this method than mapping the memory to perform the operation virtually.

## See Also

### Operating on the Memory

- performOperation

Perform an operation on the memory descriptor's memory.

- dmaCommandOperation

