

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOInterruptEventSource
-  warmCPU 

# warmCPU

Tries to reduce latency for an interrupt which will be received near a specified time.

``` source
IOReturn warmCPU(
 uint64_tabstime); 
```

## Parameters 

`abstime`  

Time at which interrupt is expected.

## Overview

Warms up a CPU in advance of an interrupt so that the interrupt may be serviced with predictable latency. The warm-up is not periodic; callers should call warmCPU once in advance of each interrupt. It is recommended that requests be issues in serial (i.e. each after the target for the previous call has elapsed), as there is a systemwide cap on the number of outstanding requests. This routine may be disruptive to the system if used with very small intervals between requests; it should be used only in cases where interrupt latency is absolutely critical, and tens or hundreds of milliseconds between targets is the expected time scale. NOTE: it is not safe to call this method with interrupts disabled.

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

normalInterruptOccurred

Functions that get called by the interrupt controller.See \$link IOService::registerInterrupt

setWorkLoop

Sub-class implementation of setWorkLoop method.

