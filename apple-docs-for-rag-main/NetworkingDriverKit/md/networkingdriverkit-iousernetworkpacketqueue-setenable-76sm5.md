

- NetworkingDriverKit
- IOUserNetworkPacketQueue
-  SetEnable 

Instance Method

# SetEnable

Enables or disables the queue.

DriverKit

``` source
kern_return_t SetEnable(bool isEnable);
```

## Parameters 

`isEnable`  

If `YES`, prepare the queue to run.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

