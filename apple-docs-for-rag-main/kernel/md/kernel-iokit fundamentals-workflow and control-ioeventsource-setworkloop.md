

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOEventSource
-  setWorkLoop 

# setWorkLoop

Set'ter for \$link workLoop variable.

``` source
virtual void setWorkLoop(
 IOWorkLoop *workLoop); 
```

## Parameters 

`workLoop`  

Target work-loop of this event source instance. A subclass of IOWorkLoop that at least reacts to signalWorkAvailable() and onThread functions.

## See Also

### Miscellaneous

checkForWork

Virtual member function used by IOWorkLoop for work scheduling.

disable

Disable event source.

enable

Enable event source.

getAction

Get'ter for \$link action variable.

getNext

Get'ter for \$link eventChainNext variable.

getWorkLoop

Get'ter for \$link workLoop variable.

init

Primary initialiser for the IOEventSource class.

isEnabled

Get'ter for \$link enable variable.

onThread

Convenience function for workLoop-\>onThread.

setAction

Set'ter for \$link action variable.

setNext

Set'ter for \$link eventChainNext variable.

