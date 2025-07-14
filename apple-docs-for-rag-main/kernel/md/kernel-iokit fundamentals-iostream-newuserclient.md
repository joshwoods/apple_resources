

- Kernel
- IOKit Fundamentals
- IOStream
-  newUserClient 

# newUserClient

See the documentation for the IOService method newUserClient.

``` source
virtual IOReturn newUserClient(
 task_t owningTask,
 void *securityID, 
 UInt32 type,
 OSDictionary *properties, 
 IOUserClient **handler ); 
```

