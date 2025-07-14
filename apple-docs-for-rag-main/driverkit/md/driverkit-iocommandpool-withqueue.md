

- DriverKit
- IOCommandPool
-  withQueue 

Static Method

# withQueue

DriverKitiOSiPadOSmacOS

``` source
static IOCommandPoolPtr withQueue(IODispatchQueue * queue);
```

## Parameters 

`queue`  

The IODispatchQueue that this command pool should synchronize with. This queue must have been allocated with the kIODispatchQueueReentrant option. Returns a pointer to an instance of IOCommandPool if successful, otherwise NULL.

## Discussion

```
         a new instance of an IOCommandPool and returns a pointer to that object.
```

