

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOCommandPool
-  initWithWorkLoop 

# initWithWorkLoop

Primary initializer for an IOCommandPool object.

``` source
virtual bool initWithWorkLoop(
 IOWorkLoop *inWorkLoop); 
```

## Parameters 

`inWorkLoop`  

The workloop that this command pool should synchronize with.

## Return Value

Returns true if command pool was successfully initialized.

## Overview

Primary initializer for an IOCommandPool. Should probably use IOCommandPool::withWorkLoop() as it is easier to use.

## See Also

### Miscellaneous

commandPool

Should never be used, obsolete. See IOCommandPool::withWorkLoop.

gatedGetCommand

gatedReturnCommand

getCommand

init

Should never be used, obsolete. See initWithWorkLoop.

returnCommand

withWorkLoop(IOService *, IOWorkLoop *, UInt32)

Should never be used, obsolete. See IOCommandPool::withWorkLoop.

withWorkLoop(IOWorkLoop *)

Primary factory method for the IOCommandPool class

