

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOCommandPool
-  getCommand 

# getCommand

``` source
virtual IOCommand *getCommand(
 bool blockForCommand = true); 
```

## Parameters 

`blockForCommand`  

If the caller would like to have its thread slept until a command is available, it should pass true, else false.

## Return Value

If the caller passes true in blockForCommand, getCommand guarantees that the result will be a pointer to an IOCommand object from the pool. If the caller passes false, s/he is responsible for checking whether a non-NULL pointer was returned.

## Overview

The getCommand method is used to get a pointer to an object of type IOCommand from the pool.

## See Also

### Miscellaneous

commandPool

Should never be used, obsolete. See IOCommandPool::withWorkLoop.

gatedGetCommand

gatedReturnCommand

init

Should never be used, obsolete. See initWithWorkLoop.

initWithWorkLoop

Primary initializer for an IOCommandPool object.

returnCommand

withWorkLoop(IOService *, IOWorkLoop *, UInt32)

Should never be used, obsolete. See IOCommandPool::withWorkLoop.

withWorkLoop(IOWorkLoop *)

Primary factory method for the IOCommandPool class

