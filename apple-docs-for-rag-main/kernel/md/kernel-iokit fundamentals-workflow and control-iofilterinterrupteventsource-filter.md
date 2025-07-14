

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOFilterInterruptEventSource
-  Filter 

# Filter

``` source
typedef bool ( *Filter)(
   OSObject *,
   IOFilterInterruptEventSource *);
```

## Parameters 

`owner`  

Pointer to the owning/client instance.

`sender`  

Where is the interrupt comming from.

## Return Value

false if this interrupt can be ignored.

## Overview

C Function pointer to a routine to call when an interrupt occurs.

