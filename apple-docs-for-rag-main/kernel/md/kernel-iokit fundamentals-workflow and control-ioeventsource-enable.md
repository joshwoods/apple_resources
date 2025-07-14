

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOEventSource
-  enable 

# enable

Enable event source.

``` source
virtual void enable(); 
```

## Overview

A subclass implementation is expected to respect the enabled state when checkForWork is called. Calling this function will cause the work-loop to be signalled so that a checkForWork is performed.

## See Also

### Miscellaneous

checkForWork

Virtual member function used by IOWorkLoop for work scheduling.

disable

Disable event source.

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

