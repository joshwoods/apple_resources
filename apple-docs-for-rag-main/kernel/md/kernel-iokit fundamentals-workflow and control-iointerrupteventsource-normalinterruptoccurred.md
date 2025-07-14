

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOInterruptEventSource
-  normalInterruptOccurred 

# normalInterruptOccurred

Functions that get called by the interrupt controller.See \$link IOService::registerInterrupt

``` source
virtual void normalInterruptOccurred(
 void *,
 IOService *nub,
 intind); 
```

## Parameters 

`nub`  

Where did the interrupt originate from

`ind`  

What is this interrupts index within 'nub'.

## See Also

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

setWorkLoop

Sub-class implementation of setWorkLoop method.

warmCPU

Tries to reduce latency for an interrupt which will be received near a specified time.

