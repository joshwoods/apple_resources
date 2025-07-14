

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOCommandPool
-  returnCommand 

# returnCommand

``` source
virtual void returnCommand(
 IOCommand *commmand); 
```

## Parameters 

`commmand`  

The command to place in the pool.

## Overview

The returnCommand method is used to place an object of type IOCommand into the pool, whether it be the first time, or the 1000th time.

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

withWorkLoop(IOService *, IOWorkLoop *, UInt32)

Should never be used, obsolete. See IOCommandPool::withWorkLoop.

withWorkLoop(IOWorkLoop *)

Primary factory method for the IOCommandPool class

