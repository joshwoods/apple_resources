

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOInterruptEventSource
-  checkForWork 

# checkForWork

Pure Virtual member function used by IOWorkLoop for issueing a client calls.

``` source
virtual bool checkForWork(); 
```

## Return Value

Return true if this function needs to be called again before all its outstanding events have been processed.

## Overview

This function called when the work-loop is ready to check for any work to do and then to call out the owner/action.

## See Also

### Miscellaneous

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

