

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOCommandPool
-  commandPool 

# commandPool

Should never be used, obsolete. See IOCommandPool::withWorkLoop.

``` source
static IOCommandPool *commandPool(
 IOService *inOwner, 
 IOWorkLoop *inWorkLoop, 
 UInt32 inSize = kIOCommandPoolDefaultSize); 
```

## See Also

### Miscellaneous

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

withWorkLoop(IOWorkLoop *)

Primary factory method for the IOCommandPool class

