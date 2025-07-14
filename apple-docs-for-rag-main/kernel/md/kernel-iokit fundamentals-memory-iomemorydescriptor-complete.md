

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  complete 

# complete

Complete processing of the memory after an I/O transfer finishes.

``` source
virtual IOReturn complete(
 IODirection forDirection = forDirection) = 0; 
```

## Parameters 

`forDirection`  

DEPRECATED The direction of the I/O just completed, or kIODirectionNone for the direction specified by the memory descriptor.

## Return Value

An IOReturn code.

## Overview

This method should not be called unless a prepare was previously issued; the prepare() and complete() must occur in pairs, before and after an I/O transfer involving pageable memory. In 10.3 or greater systems the direction argument to complete is not longer respected. The direction is totally determined at prepare() time.

## See Also

### Preparing the Buffer

prepare

Prepare the memory for an I/O transfer.

- prepare

Prepare the memory for an I/O transfer.

- complete

Complete processing of the memory after an I/O transfer finishes.

- getPreparationID

- setPreparationID

