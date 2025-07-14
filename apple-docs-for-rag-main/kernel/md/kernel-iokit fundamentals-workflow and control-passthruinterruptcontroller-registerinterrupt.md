

- Kernel
- IOKit Fundamentals
- Workflow and Control
- PassthruInterruptController
-  registerInterrupt 

Instance Method

# registerInterrupt

macOS 11.0+

``` source
virtual IOReturn registerInterrupt(IOService *nub, int source, void *target, IOInterruptHandler handler, void *refCon);
```

