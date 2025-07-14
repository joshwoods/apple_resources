

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOCommandPool
-  withWorkLoop(IOWorkLoop \*) 

# withWorkLoop(IOWorkLoop \*)

Primary factory method for the IOCommandPool class

``` source
static IOCommandPool *withWorkLoop(
 IOWorkLoop *inWorkLoop); 
```

## Parameters 

`inWorkLoop`  

The workloop that this command pool should synchronize with.

## Return Value

Returns a pointer to an instance of IOCommandPool if successful, otherwise NULL.

## Overview

The withWorkLoop method is what is known as a factory method. It creates a new instance of an IOCommandPool and returns a pointer to that object.

## See Also

### Miscellaneous

commandPool

Should never be used, obsolete. See IOCommandPool::withWorkLoop.

gatedGetCommand

gatedReturnCommand

getCommand

init

Should never be used, obsolete. See initWithWorkLoop.

initWithWorkLoop

Primary initializer for an IOCommandPool object.

returnCommand

withWorkLoop(IOService *, IOWorkLoop *, UInt32)

Should never be used, obsolete. See IOCommandPool::withWorkLoop.

