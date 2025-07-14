

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOEventSource
-  getWorkLoop 

# getWorkLoop

Get'ter for \$link workLoop variable.

``` source
virtual IOWorkLoop *getWorkLoop() const; 
```

## Return Value

value of workLoop.

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

