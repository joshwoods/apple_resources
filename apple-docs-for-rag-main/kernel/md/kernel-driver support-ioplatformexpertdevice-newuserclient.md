

- Kernel
- Driver Support
- IOPlatformExpertDevice
-  newUserClient 

Instance Method

# newUserClient

macOS 10.11.4+

``` source
virtual IOReturn newUserClient(task_t owningTask, void *securityID, UInt32 type, OSDictionary *properties, IOUserClient **handler);
```

