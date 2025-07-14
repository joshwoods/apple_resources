

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOInterruptEventSource
-  init 

# init

Primary initialiser for the IOInterruptEventSource class.

``` source
virtual bool init(
 OSObject *owner, 
 Action action, 
 IOService *provider = 0, 
 int intIndex = 0); 
```

## Parameters 

`owner`  

Owning client of the new event source.

`action`  

'C' Function to call when something happens.

`provider`  

IOService that represents the interrupt source. Defaults to 0. When no provider is defined the event source assumes that the client will in some manner call the interruptOccured method explicitly. This will start the ball rolling for safe delivery of asynchronous event's into the driver.

`intIndex`  

The index of the interrupt within the provider's interrupt sources. Defaults to 0, i.e. the first interrupt in the provider.

## Return Value

true if the inherited classes and this instance initialise successfully.

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

