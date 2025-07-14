

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOInterruptEventSource
-  getAutoDisable 

# getAutoDisable

Get'ter for \$link autoDisable variable.

``` source
virtual bool getAutoDisable() const; 
```

## Return Value

value of autoDisable.

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

