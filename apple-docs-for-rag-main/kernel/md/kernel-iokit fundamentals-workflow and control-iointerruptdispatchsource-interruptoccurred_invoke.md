

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOInterruptDispatchSource
-  InterruptOccurred_Invoke 

Type Method

# InterruptOccurred_Invoke

macOS 15.4+

``` source
static kern_return_t InterruptOccurred_Invoke(const IORPC rpc, OSMetaClassBase *target, InterruptOccurred_Handler func);
```

