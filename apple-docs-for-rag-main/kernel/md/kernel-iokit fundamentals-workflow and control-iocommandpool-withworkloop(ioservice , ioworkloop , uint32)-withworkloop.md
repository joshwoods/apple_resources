

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOCommandPool
-  withWorkLoop(IOService \*, IOWorkLoop \*, UInt32) 

# withWorkLoop(IOService \*, IOWorkLoop \*, UInt32)

Should never be used, obsolete. See IOCommandPool::withWorkLoop.

``` source
static IOCommandPool *commandPool(
 IOService *inOwner, 
 IOWorkLoop *inWorkLoop, 
 UInt32 inSize = kIOCommandPoolDefaultSize); 
```

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

withWorkLoop(IOWorkLoop *)

Primary factory method for the IOCommandPool class

