

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOFilterInterruptEventSource 

Class

# IOFilterInterruptEventSource

Filtering varient of the \$link IOInterruptEventSource.

macOS 10.0+

``` source
class IOFilterInterruptEventSource : IOInterruptEventSource
```

## Overview

An interrupt event source that calls the client to determine if a interrupt event needs to be scheduled on the work loop. A filter interrupt event source call's the client in the primary interrupt context, the client can then interrogate its hardware and determine if the interrupt needs to be processed yet.

As the routine is called in the primary interrupt context great care must be taken in the writing of this routine. In general none of the generic IOKit environment is safe to call in this context. We intend this routine to be used by hardware that can interrogate its registers without destroying state. Primarily this variant of event sources will be used by drivers that share interrupts. The filter routine will determine if the interrupt is a real interrupt or a ghost and thus optimise the work thread context switch away.

If you are implementing 'SoftDMA' (or pseudo-DMA), you may not want the I/O Kit to automatically start your interrupt handler routine on your work loop when your filter routine returns true. In this case, you may choose to have your filter routine schedule the work on the work loop itself and then return false. If you do this, the interrupt will not be disabled in hardware and you could receive additional primary interrupts before your work loop–level service routine completes. Because this scheme has implications for synchronization between your filter routine and your interrupt service routine, you should avoid doing this unless your driver requires SoftDMA.

CAUTION: Called in primary interrupt context, if you need to disable interrupt to guard you registers against an unexpected call then it is better to use a straight IOInterruptEventSource and its secondary interrupt delivery mechanism.

## Topics

### Miscellaneous

disableInterruptOccurred

Override \$link IOInterruptEventSource::disableInterruptOccurred to make a filter callout.

filterInterruptEventSource

Factor method to create and initialise an IOFilterInterruptEventSource. See \$link init.

getFilterAction

Get'ter for filterAction variable.

init

Primary initialiser for the IOFilterInterruptEventSource class.

normalInterruptOccurred

Override \$link IOInterruptEventSource::normalInterruptOccured to make a filter callout.

signalInterrupt

Cause the work loop to schedule the action.

### Callbacks

Filter

### Constants

Miscellaneous Defines

### DataTypes

ExpansionData

### Instance Variables

reserved

filterAction

### Instance Methods

- disableInterruptOccurred

- free

- getFilterAction

- getFilterActionBlock

- getMetaClass

- init

- init

- normalInterruptOccurred

- signalInterrupt

### Type Methods

+ filterInterruptEventSource

+ filterInterruptEventSource

+ interruptEventSource

## Relationships

### Inherits From

- IOInterruptEventSource

## See Also

### Interrupts

IOInterruptDispatchSource

IOInterruptDispatchSourceInterface

IOInterruptEventSource

Event source for interrupt delivery to work-loop based drivers.

IOInterruptController

PassthruInterruptController

IOInterruptSource

IOInterruptVector

