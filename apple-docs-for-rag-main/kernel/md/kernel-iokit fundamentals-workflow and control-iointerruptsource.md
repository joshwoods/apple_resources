

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOInterruptSource 

Structure

# IOInterruptSource

macOS 10.0+

``` source
typedef struct IOInterruptSource {
    ...
} IOInterruptSource;
```

## Topics

### Instance Properties

interruptController

vectorData

## See Also

### Interrupts

IOInterruptDispatchSource

IOInterruptDispatchSourceInterface

IOFilterInterruptEventSource

Filtering varient of the \$link IOInterruptEventSource.

IOInterruptEventSource

Event source for interrupt delivery to work-loop based drivers.

IOInterruptController

PassthruInterruptController

IOInterruptVector

