

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOEventSource
-  checkForWork 

# checkForWork

Virtual member function used by IOWorkLoop for work scheduling.

``` source
virtual bool checkForWork(); 
```

## Return Value

Return true if this function needs to be called again before all its outstanding events have been processed.

## Overview

This function will be called to request a subclass to check its internal state for any work to do and then to call out the owner/action. If this event source never performs any work (e.g. IOCommandGate), this method should not be overridden. NOTE: This method is no longer declared pure virtual. A default implementation is provided in IOEventSource.

## See Also

### Miscellaneous

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

setWorkLoop

Set'ter for \$link workLoop variable.

