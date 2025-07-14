

- Kernel
- IOKit Fundamentals
- IOService
-  newUserClient 

Instance Method

# newUserClient

macOS 11.0+

``` source
IOReturn newUserClient(task_t owningTask, void *securityID, UInt32 type, OSDictionary *properties, OSSharedPtr & handler);
```

