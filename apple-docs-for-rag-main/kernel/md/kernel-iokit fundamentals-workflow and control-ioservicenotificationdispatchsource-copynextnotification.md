

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOServiceNotificationDispatchSource
-  CopyNextNotification 

Instance Method

# CopyNextNotification

macOS 10.15.4+

``` source
kern_return_t CopyNextNotification(uint64_t *type, IOService **service, uint64_t *options, OSDispatchMethod supermethod);
```

