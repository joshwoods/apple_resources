

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOEventSource
-  onThread 

# onThread

Convenience function for workLoop-\>onThread.

``` source
virtual bool onThread() const; 
```

## Return Value

true if called on the work-loop thread.

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

setAction

Set'ter for \$link action variable.

setNext

Set'ter for \$link eventChainNext variable.

setWorkLoop

Set'ter for \$link workLoop variable.

