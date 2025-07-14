

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOInterruptController
-  registerInterrupt 

Instance Method

# registerInterrupt

macOS 10.11.4+

``` source
virtual IOReturn registerInterrupt(IOService *nub, int source, void *target, IOInterruptHandler handler, void *refCon);
```

