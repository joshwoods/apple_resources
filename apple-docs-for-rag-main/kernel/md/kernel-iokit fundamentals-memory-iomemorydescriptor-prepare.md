

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  prepare 

# prepare

Prepare the memory for an I/O transfer.

``` source
virtual IOReturn prepare(
 IODirection forDirection = forDirection) = 0; 
```

## Parameters 

`forDirection`  

The direction of the I/O just completed, or kIODirectionNone for the direction specified by the memory descriptor.

## Return Value

An IOReturn code.

## Overview

This involves paging in the memory, if necessary, and wiring it down for the duration of the transfer. The complete() method completes the processing of the memory after the I/O transfer finishes. Note that the prepare call is not thread safe and it is expected that the client will more easily be able to guarantee single threading a particular memory descriptor.

## See Also

### Preparing the Buffer

- prepare

Prepare the memory for an I/O transfer.

complete

Complete processing of the memory after an I/O transfer finishes.

- complete

Complete processing of the memory after an I/O transfer finishes.

- getPreparationID

- setPreparationID

