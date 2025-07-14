

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOInterruptVector 

Structure

# IOInterruptVector

macOS 10.0+

``` source
typedef struct IOInterruptVector {
    ...
} IOInterruptVector;
```

## Topics

### Instance Properties

handler

interruptActive

interruptDisabledHard

interruptDisabledSoft

interruptLock

interruptRegistered

nub

refCon

sharedController

source

target

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

IOInterruptSource

