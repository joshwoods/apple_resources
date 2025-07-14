

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  PassthruInterruptController 

Class

# PassthruInterruptController

macOS 11.0+

``` source
class PassthruInterruptController : IOInterruptController
```

## Topics

### Instance Methods

- causeInterrupt

- disableInterrupt

- enableInterrupt

- externalInterrupt

- getInterruptType

- getMetaClass

- handleInterrupt

- init

- registerInterrupt

- setCPUInterruptProperties

- waitForChildController

## Relationships

### Inherits From

- IOInterruptController

## See Also

### Interrupts

IOInterruptDispatchSource

IOInterruptDispatchSourceInterface

IOFilterInterruptEventSource

Filtering varient of the \$link IOInterruptEventSource.

IOInterruptEventSource

Event source for interrupt delivery to work-loop based drivers.

IOInterruptController

IOInterruptSource

IOInterruptVector

