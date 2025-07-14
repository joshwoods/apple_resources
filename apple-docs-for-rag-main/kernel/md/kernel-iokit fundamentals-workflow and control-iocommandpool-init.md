

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOCommandPool
-  init 

# init

Should never be used, obsolete. See initWithWorkLoop.

``` source
virtual bool init(
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

initWithWorkLoop

Primary initializer for an IOCommandPool object.

returnCommand

withWorkLoop(IOService *, IOWorkLoop *, UInt32)

Should never be used, obsolete. See IOCommandPool::withWorkLoop.

withWorkLoop(IOWorkLoop *)

Primary factory method for the IOCommandPool class

