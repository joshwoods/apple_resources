

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOInterruptEventSource 

Class

# IOInterruptEventSource

Event source for interrupt delivery to work-loop based drivers.

macOS 10.0+

``` source
class IOInterruptEventSource : IOEventSource
```

## Overview

The IOInterruptEventSource is a generic object that delivers calls interrupt routines in it's client in a guaranteed single-threaded manner. IOInterruptEventSource is part of the IOKit \$link IOWorkLoop infrastructure where the semantic that one and only one action method is executing within a work-loops event chain.

When the action method is called in the client member function will receive 2 arguments, (IOEventSource \*) sender and (int) count, See \$link IOInterruptEventSource::Action. Where sender will be reference to the interrupt that occurred and the count will be computed by the difference between the \$link producerCount and \$link consumerCount. This number may not be reliable as no attempt is made to adjust for around the world type problems but is provided for general information and statistic gathering.

In general a client will use the factory member function to create and initialise the event source and then add it to their work-loop. It is the work loop's responsiblity to maintain the new event source in it's event chain. See \$link IOWorkLoop.

An interrupt event source attaches itself to the given provider's interrupt source at initialisation time. At this time it determines if it is connected to a level or edge triggered interrupt. If the interrupt is an level triggered interrupt the event source automatically disables the interrupt source at primary interrupt time and after it call's the client it automatically reenables the interrupt. This action is fairly expensive but it is 100% safe and defaults sensibly so that the driver writer does not have to implement type dependant interrupt routines. So to repeat, the driver writer does not have to be concerned by the actual underlying interrupt mechanism as the event source hides the complexity.

Saying this if the hardware is a multi-device card, for instance a 4 port NIC, where all of the devices are sharing one level triggered interrupt AND it is possible to determine each port's interrupt state non-destructively then the \$link IOFilterInterruptEventSource would be a better choice.

Warning: All IOInterruptEventSources are created in the disabled state. If you want to actually schedule interrupt delivery do not forget to enable the source.

## Topics

### Miscellaneous

checkForWork

Pure Virtual member function used by IOWorkLoop for issueing a client calls.

disable

Disable event source.

disableInterruptOccurred

Functions that get called by the interrupt controller.See \$link IOService::registerInterrupt

enable

Enable event source.

free

Sub-class implementation of free method, disconnects from the interrupt source.

getAutoDisable

Get'ter for \$link autoDisable variable.

getIntIndex

Get'ter for \$link intIndex interrupt index variable.

getProvider

Get'ter for \$link provider variable.

init

Primary initialiser for the IOInterruptEventSource class.

interruptEventSource

Factory function for IOInterruptEventSources creation and initialisation.

interruptOccurred

Functions that get called by the interrupt controller. See \$link IOService::registerInterrupt

normalInterruptOccurred

Functions that get called by the interrupt controller.See \$link IOService::registerInterrupt

setWorkLoop

Sub-class implementation of setWorkLoop method.

warmCPU

Tries to reduce latency for an interrupt which will be received near a specified time.

### Callbacks

Action

### Constants

Miscellaneous Defines

### DataTypes

ExpansionData

### Instance Variables

reserved

provider

producerCount

intIndex

explicitDisable

consumerCount

autoDisable

### Instance Methods

- checkForWork

- disable

- disableInterruptOccurred

- enable

- enablePrimaryInterruptTimestamp

- free

- getAutoDisable

- getIntIndex

- getMetaClass

- getPrimaryInterruptTimestamp

- getProvider

- init

- interruptOccurred

- normalInterruptOccurred

- registerInterruptHandler

- setWorkLoop

- unregisterInterruptHandler

- warmCPU

### Type Methods

+ interruptEventSource

+ interruptEventSource

## Relationships

### Inherits From

- IOEventSource

## See Also

### Interrupts

IOInterruptDispatchSource

IOInterruptDispatchSourceInterface

IOFilterInterruptEventSource

Filtering varient of the \$link IOInterruptEventSource.

IOInterruptController

PassthruInterruptController

IOInterruptSource

IOInterruptVector

