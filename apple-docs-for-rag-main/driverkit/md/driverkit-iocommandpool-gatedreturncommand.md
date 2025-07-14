

- DriverKit
- IOCommandPool
-  gatedReturnCommand 

Instance Method

# gatedReturnCommand

DriverKitiOSiPadOSmacOS

``` source
kern_return_t gatedReturnCommand(IOCommand * command);
```

## Parameters 

`command`  

A pointer to the IOCommand object to be returned to the pool.

## Return Value

kIOReturnSuccess on success. See IOReturn.h for error codes.

## Discussion

The gatedReturnCommand method is used to serialize the return of a command to the pool synchronized with the pool’s queue.

