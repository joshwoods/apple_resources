

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOFilterInterruptEventSource
-  filterInterruptEventSource 

Type Method

# filterInterruptEventSource

macOS 10.15.2+

``` source
static OSPtr filterInterruptEventSource(OSObject *owner, IOService *provider, int intIndex, IOInterruptEventSource::ActionBlock action, FilterBlock filter);
```

