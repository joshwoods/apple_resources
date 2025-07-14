

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOCommandPool
-  gatedReturnCommand 

# gatedReturnCommand

``` source
virtual IOReturn gatedReturnCommand(
 IOCommand *vCommand); 
```

## Parameters 

`vCommand`  

A pointer to the IOCommand object to be returned to the pool.

## Return Value

Always returns kIOReturnSuccess if the vCommand argument is valid.

## Overview

The gatedReturnCommand method is used to serialize the return of a command to the pool behind a command gate, runAction-ed by returnCommand.

## See Also

### Miscellaneous

commandPool

Should never be used, obsolete. See IOCommandPool::withWorkLoop.

gatedGetCommand

getCommand

init

Should never be used, obsolete. See initWithWorkLoop.

initWithWorkLoop

Primary initializer for an IOCommandPool object.

returnCommand

withWorkLoop(IOService *, IOWorkLoop *, UInt32)

Should never be used, obsolete. See IOCommandPool::withWorkLoop.

withWorkLoop(IOWorkLoop *)

Primary factory method for the IOCommandPool class

