

- DriverKit
- IOCommandPool
-  initWithQueue 

Instance Method

# initWithQueue

DriverKitiOSiPadOSmacOS

``` source
bool initWithQueue(IODispatchQueue * queue);
```

## Parameters 

`queue`  

The IODispatchQueue that this command pool should synchronize with. This queue must have been allocated with the kIODispatchQueueReentrant option.

## Return Value

Returns true if command pool was successfully initialized.

## Discussion

```
         Should probably use IOCommandPool::withQueue() as it is easier to use.
```

