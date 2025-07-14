

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOCommandPool
-  gatedGetCommand 

# gatedGetCommand

``` source
virtual IOReturn gatedGetCommand(
 IOCommand **vCommand,
 boolvBlock); 
```

## Parameters 

`vCommand`  

A pointer to a pointer to an IOCommand object where the returned command will be stored.

`vBlock`  

A bool that indicates whether to block the request until a command becomes available.

## Return Value

Returns kIOReturnNoResources if no command is available and the client doesn't wish to block until one does become available. kIOReturnSuccess if the vCommand argument is valid.

## Overview

The gatedGetCommand method is used to serialize the extraction of a command from the pool behind a command gate, runAction-ed by getCommand.

## See Also

### Miscellaneous

commandPool

Should never be used, obsolete. See IOCommandPool::withWorkLoop.

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

