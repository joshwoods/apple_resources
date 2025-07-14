

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOInterruptController 

Class

# IOInterruptController

macOS 10.0+

``` source
class IOInterruptController : IOService
```

## Topics

### Instance Methods

- cancelDeferredIPI

- causeInterrupt

- causeVector

- disableInterrupt

- disableVectorHard

- enableInterrupt

- enableVector

- getInterruptHandlerAddress

- getInterruptType

- getMetaClass

- getVectorType

- handleInterrupt

- initVector

- registerInterrupt

- sendIPI

- setCPUInterruptProperties

- timeStampInterruptHandlerEnd

- timeStampInterruptHandlerInternal

- timeStampInterruptHandlerStart

- timeStampSpuriousInterrupt

- unregisterInterrupt

- vectorCanBeShared

## Relationships

### Inherits From

- IOService

## See Also

### Interrupts

IOInterruptDispatchSource

IOInterruptDispatchSourceInterface

IOFilterInterruptEventSource

Filtering varient of the \$link IOInterruptEventSource.

IOInterruptEventSource

Event source for interrupt delivery to work-loop based drivers.

PassthruInterruptController

IOInterruptSource

IOInterruptVector

